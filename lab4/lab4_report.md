University: [ITMO University](https://itmo.ru/ru/)\
Faculty: [FICT](https://fict.itmo.ru)\
Course: IP-telephony\
Year: 2022/2023\
Group: K34202\
Author: Sidorenko Darya Alekseevna\
Lab: Lab1\
Date of create: 31.03.2023\
Date of finished: \
Цель:
Изучить построение сети IP-телефонии между удаленными филиалами с помощью маршрутизаторов Cisco 2811 и коммутаторов Cisco 2950Т. \
Ход работы:
## Часть 1
+ В рабочей среде Cisco Packet Tracer собрана схема соединения согласно требованиям. В конфигурационном режиме изменено название маршрутизаторов на RouterA, RouterB. \
![image](https://user-images.githubusercontent.com/80837580/229056056-94d77fa7-1e64-4825-9785-e79e1556d72b.png)
+ Проведена конфигурация интерфейса fa0/0 на роутере RouterA.\
![image](https://user-images.githubusercontent.com/80837580/229049479-99783e3e-530e-41c9-95ef-1c84e81baa4e.png)
+ Проведена конфигурация интерфейса fa0/0 на роутере RouterB.\
![image](https://user-images.githubusercontent.com/80837580/229049757-49942626-32fb-4b66-8de6-6a3af39ed9c5.png)
+ Проведена конфигурация интерфейса s0/3/0 на обоих маршрутизаторах. \
![image](https://user-images.githubusercontent.com/80837580/229050266-2bd55811-c6af-48b9-b916-495efd4a1d2d.png) \
![image](https://user-images.githubusercontent.com/80837580/229050594-3afe7128-ab4f-4497-99ec-95418e36d0f7.png)
+ Для обоих маршрутизаторов был настроен DHCP сервер. Создан пул DHCP адреса, задана сеть, в которой будет работать DHCP сервер, указан ip адрес нужного VLAN. Опция 150 использована для того, чтобы IP-телефоны использовали настройки CallManager Express с TFTP сервера. \
![image](https://user-images.githubusercontent.com/80837580/229051543-a72ae99a-f38e-4d28-b1a5-0b7ee856ca63.png)\
![image](https://user-images.githubusercontent.com/80837580/229051970-bedab15a-0ef3-443a-a603-1d2468c169b8.png)
+ Выполенна настройка динамической маршрутизации на основе протокола RIP для передачи информации между маршрутизаторами в сети.\
![image](https://user-images.githubusercontent.com/80837580/229052185-d6156b96-475f-4899-bbf0-8160cbd942c7.png)\
![image](https://user-images.githubusercontent.com/80837580/229052494-d248900a-15e7-43ee-9070-2db8d001881f.png)
+ Выполнена настройка телефонного сервиса CallManager Express.\
![image](https://user-images.githubusercontent.com/80837580/229052873-9bc3ec7d-4325-4454-8706-246e247c87e0.png)\
![image](https://user-images.githubusercontent.com/80837580/229053201-96528f4b-4c03-4b81-88e7-62aa72373c25.png)
+ На коммутаторе назначен даипазон портов. \
![image](https://user-images.githubusercontent.com/80837580/229054001-578eb49d-25ad-47bb-8ca7-ef325679f3c2.png)
+ Проведена настройка IP-телефонов.\
![image](https://user-images.githubusercontent.com/80837580/229054709-3a2b40aa-1235-4ac0-bf2b-729fc468211f.png)\
![image](https://user-images.githubusercontent.com/80837580/229055003-635a5ba6-c63b-4d97-8858-86d38db38107.png)
+ Настроена передача звонков между удаленными сетями\
![image](https://user-images.githubusercontent.com/80837580/229055245-16e52c1f-46ba-4b13-b8f1-d76f418653aa.png)\
![image](https://user-images.githubusercontent.com/80837580/229055577-acc461b6-94c4-4f43-bf4a-41856c97bfc8.png)
+ Корректность связи проверена. \
![1234](https://user-images.githubusercontent.com/80837580/229059443-94a87729-1e1e-4a74-ac17-4c917218af1b.png)\
![1](https://user-images.githubusercontent.com/80837580/229057535-4e6a1c31-da46-4a68-af36-36c1e26f0239.png)






