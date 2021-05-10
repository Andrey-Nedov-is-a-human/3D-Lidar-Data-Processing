# Обработка данных 3D-лидара, отслеживание объектов и расчёт коридора проходимости робота / Processing 3D lidar data, tracking objects and calculating the passageway of the robot

<img src="/imgs/img4.png" alt="img1" width="700"/>

*Разработчики/Developers*
1. [Андрей Недов](https://github.com/Andrey-Nedov-is-a-human)

# Задача

_Разработать алгоритм считывания и визуализации потоковых данных в виде динамически обновляемого облака точек многолучевого 3D-лидара._

- Подготовить приложение считывания данных с 3D-лидара, сохраненных в файле потоковом формате и вычисления облака точек; 
- Разработать функцию динамического обновления данных в заданной структуре (объекте) для хранения данных облака точек; 
- Разработать функцию покадровой визуализации облака точек в изометрической проекции и в режиме «вид сверху» с заданным (настраиваемым) фреймрейтом (частотой); 
- Разработать функцию фильтрации данных с использованием плоскостей отсечения (куб интереса); 
- Разработать функцию детектирования объектов методом кластерного анализа;
- Разработать метод отслеживания «коридора проходимости» для прямолинейного движения робота.

# Лидар

В работе использовались сырые данные, записанные с 32-лучевого 3D-лидара Velodyne HDL-32E.

[Спецификация/Specification](https://github.com/Andrey-Nedov-is-a-human/3D-Lidar-Data-Processing/tree/main/materials/Velodyne_techinfo.pdf)

<img src="/imgs/lidar.jpg" width="700"/>

# Результат

[Видеоотчёт/Video report](https://drive.google.com/drive/u/0/folders/1VZhtAhdNhnO-oVso0GQji8zkEwWhYuO_)

В 3D-пространстве робот предствлен зелёной горизонтальной плоскостью на поверхности куба отсечения. Прозрачный параллелепипед показывает коридор проходимости, доступный для беспрепятственного прямолинейного передвижения робота.

<img src="/imgs/img1.png" width="700"/>

Программа читает из файла сырые данные, записанные с лидара покетами
