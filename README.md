# Переменные и базовые типы языка
## Переменные
Программы чаще всего манипулируют данными, например расчет формул, или отображения каких либо данных на экране и т.д. Т.е. для выполнения задач над этими данными, нам необходимая некая сущность чтобы управлять этими данными, например хранить результат вычесление одной формулы и использовать как часть входных параметров для другой формулы. И этой сущностью являеться переменная. Т.е. переменная это ячейка в памяти которая предназначенна для манипуляции даными в этой ячейке, т.е. хранить или записывать данные в ячейке. Другими словами переменная это уникальное идентификатор через который мы можем сослаться на участок памяти, с которой связана переменная. Переменная это просто имя предназначеное для удобности чтения кода, при компиляции переменная это просто адресс ячейки памяти. Переменная должна удовлетворять правилам идентификаторов, которые описаны в предыдущем разделе.
Например представте вы пишете персонажа к игре, и персонаж в какойто момент времени имеет позицию на карте и персонаж может перемещаться по карте, и нам необходимо сохранять координаты персонажа в переменной, т.е. в памяти, и если нам необходимо перерисовать карту или уточнить где находиться персонаж мы можем обратиться к переменой и взять от туда текущие координаты персонажа.
Необходимо обьязательно запомнить что назначение правильного имени идентификатору, играет ключевую роль при написании приложения.
Для того что бы использовать переменную ее неободимо обьявить, для этого указывают тип переменной и ее имя, другими словами зарезервировать память под эту переменную. Почему зарезервировать, т.к. если переменная не будет использована в программе компилятор может удалить эту переменную и обьектного файла.
```cpp
// синтаксис обьявления переменной
тип_данных имя_переменной;
```
В отличие от литералов под которые не выделяется место в памяти(исключением является строковые литералы), переменные обычно храняться в стеке или куче, реже в памяти сегмента кода. При этом выделяют три вида переменных локальные, статические и динамические. В этом разделе будут в основном расматриваться локальные переменные которые будут храниться на стеке.
Если в двух словах стек это структура данных работающая по принципу LIFO(последний вошел, первый вышел), т.е. предоставляет автоматическую работу с памятью. Т.е. перемення попавшая на стек имеет предустановленное правило жизни, и вы никак не можете на это повлиять. Стек более подробно будет рссмотрен при работе с поматью.
