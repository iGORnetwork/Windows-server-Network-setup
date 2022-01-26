# Windows-server-Network-setup
## Ход выполния работы
### настройка DC1
1) Запускаем команду "выполнить" сочетанием клевать Win+R
2) В строке выполнить водим команду sconfig
3) В командной строке води цифру 2
4) Меняем имя на DC1 далее перезагружаем PC После перезагрузки выполняем 1, 2 пункт
5) водим цифру 8
6) выбираем сетевой адаптер 1
7) водим 1 и выбираем параметр S статический IP
8) водим статический ip адрес 172.16.19.65/26
9) водим маску подсети 255.255.255.192
10) водим основной шлюз 172.16.19.126
![](https://github.com/iGORnetwork/Windows-server-Network-setup/blob/main/DC1-1.png)
Протокол ICMP включен по умолчанию 
![](https://github.com/iGORnetwork/Windows-server-Network-setup/blob/main/DC1-2.png)
# настройка SRV1
1) Меняем имя - CMD - sconfig - 2 - водим имя SRV1 презагружаемся.
2) Настраеваем сеть - CMD - sconfig - 8 - 1 - 1 - S - водим IP адрес 172.16.19.66 - маска 255.255.255.192 шлюз 172.16.19.126 DNS 172.16.19.65
![](https://github.com/iGORnetwork/Windows-server-Network-setup/blob/main/SRV1-1.png)
3) Протокол ICMP включен по умолчанию 
# настройка DCA
1) Меняем имя PC WIN+r - CMD - sconfig - 2 - водим имя SRV1 презагружаемся.
2) Настраеваем сеть WIN+r - CMD - sconfig - 8 - 1 - 1 - S - водим IP адрес 172.16.19.67 - маска 255.255.255.192 шлюз 172.16.19.126 DNS 172.16.19.65
![](https://github.com/iGORnetwork/Windows-server-Network-setup/blob/main/DC1-1.png)
3) Протокол ICMP включен по умолчанию 
# настройка CLI1
1) Меняем имя PC WIN+r - CMD - sconfig - 2 - водим имя CLI1 презагружаемся.
![](https://github.com/iGORnetwork/Windows-server-Network-setup/blob/main/CLI1-1.png)
2) Протокол ICMP включен по умолчанию 
# настройка DC2
1) Меняем имя PC WIN+r - CMD - sconfig - 2 - водим имя DC2 презагружаемся.
2) Настраеваем сеть WIN+r - CMD - sconfig - 8 - 1 - 1 - S - водим IP адрес 172.16.20.97 - маска 255.255.255.224
![](https://github.com/iGORnetwork/Windows-server-Network-setup/blob/main/DC2-1.png)
3) Протокол ICMP включен по умолчанию 
# настраиваем SRV2
1) Меняем имя - CMD - sconfig - 2 - водим имя SRV2 презагружаемся.
2) Настраеваем сеть - CMD - sconfig - 8 - 1 - 1 - S - водим IP адрес 172.16.20.98 - 255.255.255.224
![](https://github.com/iGORnetwork/Windows-server-Network-setup/blob/main/SRV2-1.png)
# настройка CLI2
1) Меняем имя PC WIN+r - CMD - sconfig - 2 - водим имя CLI2 презагружаемся.
