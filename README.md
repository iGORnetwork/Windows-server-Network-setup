# Windows-server-Network-setup
## Ход выполния работы
### настройка DC1
1) Запускаем каманду "выполнить" сочетанием клевать Win+R
2) В строке выполнить водим команду sconfig
3) В командной строке води цифру 2
4) Меняем имя на DC1 далее перезагружаем PC После перезагрузки выполняем 1, 2 пункт
5) водим цифру 8
6) выбираем сетевой адаптер 1
7) водим 1 и выбираем параметр S статический IP
8) водим статический ip адрес 172.16.19.65/26
9) водим маску подсети 255.255.255.192
10) водим основной шлюз 172.16.19.126
![](DC1-1)
