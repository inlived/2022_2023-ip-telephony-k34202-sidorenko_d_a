University: [ITMO University](https://itmo.ru/ru/)\
Faculty: [FICT](https://fict.itmo.ru)\
Course: IP-telephony\
Year: 2022/2023\
Group: K34202\
Author: Sidorenko Darya Alekseevna\
Lab: Lab1\
Date of create: 28.02.2023\
Date of finished: \
Цель:
Изучить рабочую среду Cisco Packet Tracer, ознакомиться с интерфейсами основных устройств, типами кабелей, научиться собирать топологию. Изучить построение сети IP-телефонии с помощью маршрутизатора, коммутатора и IP телефонов Cisco 7960 в среде Packet tracer \
Ход работы:
## Часть 1
+ Собрана схема соединения в рабочей среде Cisco Packet Tracer согласно условиям задания.\
![image](https://user-images.githubusercontent.com/80837580/221873299-f2dede59-8b2d-4f0c-8150-d82db0225b95.png) \
+ Каждому PC присвоен IP-адрес в диапазоне 192.168.0.1-192.168.0.8 во вкладке IP-конфигурации. \
![image](https://user-images.githubusercontent.com/80837580/221874528-12b92a53-12ed-485c-a8e3-3f8253f8318d.png) \
+ Проведена проверка. Любой компьютер одной сети посредством пинга передает пакеты любому компьютеру другой сети.\
![image](https://user-images.githubusercontent.com/80837580/221875420-b268647d-7d6f-4ab1-b571-0a795ae3d051.png)\
![image](https://user-images.githubusercontent.com/80837580/221876993-99be38e9-5db3-482a-8b1e-ecc7c8999b25.png)\
## Часть 2
+ Создана новая сеть из роутера, коммутатора и двух IP-телефонов. Имя роутера Cisco 2811 изменено на CMERouter.\
![image](https://user-images.githubusercontent.com/80837580/221882028-23563e15-4264-441f-ba9f-7f2830fd90ca.png)\
+ Задан адрес маршрутизатору CMERouter, Port status ON. Оба IP-телефона подключены к сети.\
![image](https://user-images.githubusercontent.com/80837580/221881067-1a668b42-4dc2-4bf0-85f3-be90b8fbd3f8.png)\
![image](https://user-images.githubusercontent.com/80837580/221881869-156500d0-2cbd-418c-b096-c6ef97f38fc3.png)\
+ Произведена конфигурация роутера. С помощью CLI настроен dhcp для автоматической раздачи адресов конечным устройствам, загружена прошивка для телефонов, заданы основные параметры: максимально–возможное количество поддерживаемых DN (Directory Numbers - номеров), максимальное количество телефонных аппаратов, откуда наш роутер будет принимать звонки, присвоение линий в автоматическом режиме.\
![image](https://user-images.githubusercontent.com/80837580/221884249-0170648a-1ec4-497e-9700-c21a33402074.png)\
+ Настроен коммутатор. Vlan 1 выделен под VoIP с помощью CLI. \
![image](https://user-images.githubusercontent.com/80837580/221886413-11e9dc18-b38a-424a-9eac-e9c5fb3fead7.png)\
+ Телефонам назначены номера. \
![image](https://user-images.githubusercontent.com/80837580/221888885-9797404c-7d34-4128-a8ad-e575ea0fef37.png)\
+ Проведена проверка. Прозвон с одного телефона на другой прошел успешно. \
![pic1](https://user-images.githubusercontent.com/80837580/221890342-1dea2e96-df72-41da-afce-84073788daf2.png)\
Вывод: в результате выполнения работы была изучена средаCisco Packet Tracer, интерфейсы основных устройств, типы кабелей, собраны необходимые топологию. Изучено построение сети IP-телефонии с помощью маршрутизатора, коммутатора и IP телефонов Cisco 7960 в среде Packet tracer.




