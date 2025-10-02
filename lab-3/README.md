University: [ITMO University](https://itmo.ru/ru/)  
Faculty: [FICT](https://fict.itmo.ru)  
Course: [Network programming](https://github.com/itmo-ict-faculty/network-programming)  
Year: 2024/2025  
Group: K3321  
Author: Vdovina Yaroslava Dmitrievna  
Lab: Lab3  
Date of create: 02.10.2025  
Date of finished: 02.10.2025  

## Работа с NetBox
- Был развёрнут NetBox с помощью docker compose по адресу http://127.0.0.1:8000 (локально)
![Скриншот 1](images/1.jpg)
- В нетбоксе была заполнена информация о двух микротиках: Site, Tenant, Manufacturer (MikroTik), Device Type (CHR), Platform (RouterOS), Role (router), Tag (lab3)
## Ансибл сценарии
![Скриншот 4](images/4.jpg)
- nb_seed.yml — заполняет NetBox начальными объектами (site, manufacturer, device type, devices, interfaces, IP)
![Скриншот 2](images/2.png)
![Скриншот 3](images/3.png)
- nb_dump.yml — получение данных из NetBox и сохранение JSON
![Скриншот 5](images/5.png)
![Скриншот 6](images/6.png)
![Скриншот 7](images/7.png)
- nb_push_routeros.yml — строит инвентори из NetBox и конфигурирует микротик (имя устройства, IP и т.д.) по данным NetBox
![Скриншот 8](images/8.png)
![Скриншот 9](images/9.png)
- nb_pull_serial.yml —  считывает серийники с микротика и записывает их обратно в NetBox
![Скриншот 10](images/10.png)
![Скриншот 11](images/11.png)
![Скриншот 12](images/12.png)
