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
1) Меняем имя PC WIN+r - CMD - sconfig - 2 - водим имя SRV1 презагружаемся.
2) Настраеваем сеть WIN+r - CMD - sconfig - 8 - 1 - 1 - S - водим IP адрес 172.16.19.66 - маска 255.255.255.192 шлюз 172.16.19.126 DNS 172.16.19.66
3) Устанавливаем AD - WIN+r - CMD - Powershell - Install-WindowsFeature -Name AD-Domain-Services
4) Водим PC в домен WIN+r - CMD - Powershell - водим в одну строчку add-computer -domainname moscow.wsr водим пользователя и пароль, презагружаем PC
5) Возвращаемся DC1 AD идём во вкладку manage - add server - вкладка DNS и добавляем PC SRV1 и нажимаем ОК.
