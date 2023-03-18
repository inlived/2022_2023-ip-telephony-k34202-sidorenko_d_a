University: [ITMO University](https://itmo.ru/ru/)\
Faculty: [FICT](https://fict.itmo.ru)\
Course: IP-telephony\
Year: 2022/2023\
Group: K34202\
Author: Sidorenko Darya Alekseevna\
Lab: Lab1\
Date of create: 14.03.2023\
Date of finished: \
Цель:
Изучить построение сети IP-телефонии с помощью маршрутизатора Cisco 2811, коммутатора Cisco catalyst 3560 и IP телефонов Cisco 7960. \
Ход работы:
## Часть 1
+ В рабочей среде Cisco Packet Tracer собрана схема соединения согласно требованиям (маршрутизатор, коммутатор и 3 IP-телефона). В конфигурационном режиме изменено название маршрутизатора на CMERouter. С помощью CLI отключен синтаксис ввода слов от DNS серверов и заданы пароли для защиты маршрутизатора как в удаленном режиме, так и в режиме консоли.
![image](https://user-images.githubusercontent.com/80837580/226118753-5026251a-8646-45e7-bc3e-bcaed7236574.png)\
![image](https://user-images.githubusercontent.com/80837580/226118435-b9e2e3b2-ebf8-46b5-9e0b-6ff3b2c182ae.png)
+ Настроена конфигурация интерфейса fa0/0 на маршрутизаторе Cisco 2811 (CMERouter) с помощью CLI.\
![image](https://user-images.githubusercontent.com/80837580/226118536-093a9d4e-8160-469b-9710-e92b824e839d.png)
+ Настроен DHCP сервера для передачи голоса и данных на маршрутизаторе Cisco 2811. Создан пул DHCP адреса со своим названием, задана сеть, в которой будет работать DHCP сервер, указан ip адрес нужного VLAN, в данном случае для передач данных. Включена опция 150, которая нужна для того, чтобы IP-телефоны использовали настройки CallManager Express с TFTP сервера.\
![image](https://user-images.githubusercontent.com/80837580/226118690-51789456-4cb9-4e73-bd60-89a2d665810a.png)
+ Настроены услуги телефонии Cisco CallManager Express на маршрутизаторе 2811. Задано максимальное количество номеров, присваиваемых IP-телефоном, максимальное количество IP-телефонов. Задан IP адрес голосового шлюза, назначены внешние номера.\
![image](https://user-images.githubusercontent.com/80837580/226122742-0566a81a-814c-413a-9547-f0e79d8a729c.png)
+ Созданы VLAN порты на коммутаторе Cisco Catalyst 3560 для взаимодействия коммутатора с маршрутизатором и подключены IP телефоны. Для этого был настроен интерфейс управления коммутатором в сети VLAN через назначение диапазона портов. Также телефонам назначены номера в командной строке маршрутизатора.\
![image](https://user-images.githubusercontent.com/80837580/226125724-ef1b1f11-520b-4159-a0f6-b21d0983a8d3.png)\
![image](https://user-images.githubusercontent.com/80837580/226125817-5263bb27-9aa2-4963-b904-9f15c0ddd146.png)
+ Звонки между телефонами были проверены, соедиинение успешно.\
![image](https://user-images.githubusercontent.com/80837580/226125998-cbad159a-2cd5-4530-b8e8-feacbbc59ba6.png)\
![image](https://user-images.githubusercontent.com/80837580/226126055-401fc646-0315-4d92-9066-e07f1b648017.png)
## Часть 2
+ На основе схемы соединения из первой части работы получена следующая конфигурация.\
![image](https://user-images.githubusercontent.com/80837580/226127667-aefd2d1d-71a7-40b4-8f09-ce25c1a0315d.png)
+ На коммутаторе созданы vlan, им назначены наименования. Для vlan'ов созданы логические подинтерфейсы. \
![image](https://user-images.githubusercontent.com/80837580/226129080-f22688bb-dd2f-454a-9103-b70f121f38b0.png)

