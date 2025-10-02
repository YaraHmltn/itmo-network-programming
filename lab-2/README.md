University: [ITMO University](https://itmo.ru/ru/)  
Faculty: [FICT](https://fict.itmo.ru)  
Course: [Network programming](https://github.com/itmo-ict-faculty/network-programming)  
Year: 2024/2025  
Group: K3321  
Author: Vdovina Yaroslava Dmitrievna  
Lab: Lab2  
Date of create: 02.10.2025  
Date of finished: 02.10.2025  

## Настройка второго клиента в CHR
- В виртуал боксе была поднята ещё одна виртуальная машина со вторым микротиком и были повторены настройки с lab 1  
![Скриншот 1](images/1.jpg)
![Скриншот 2](images/2.jpg)
- Был создан playbook, который создаёт пользователя ансибл, включает ntp-клиент, настраивает ospf interface template для нашего соединения WG с типом ptp, открывает в firewall ospf и udp порт WG, после собирает данные об ospf топологии и полный конфиг устройств
![Скриншот 3](images/3.png)
![Скриншот 4](images/4.png)
![Скриншот 5](images/5.jpg)
![Скриншот 6](images/6.png)
- Проверка соседства на самих микротиках:  
![Скриншот 7](images/7.png)
![Скриншот 8](images/8.png)
