University: [ITMO University](https://itmo.ru/ru/) <br/>
Faculty: [FICT](https://fict.itmo.ru) <br/>
Course: IP-telephony <br/>
Year: 2022/2023 <br/>
Group: K34202 <br/>
Author: Li Galina <br/>
Lab: Lab1 <br/>
Date of create: 18.03.2023 <br/>
Date of finished: 20.03.2023 <br/>

# Лабораторная работа №2 "Конфигурация voip в среде Сisco packet tracer"

## Описание
   Для выполнения данной лабораторной работы собирается схема соединения. Необходимо проверить, правильно ли подключены все узлы устройств. Предварительно удалить все преды- дущие конфигурационные файлы на маршрутизаторах Cisco 2811, на коммутаторе Cisco catalyst 3560.
   
## Цель работы:
   Изучить построение сети IP-телефонии с помощью маршрутизатора Cisco 2811, коммутатора Cisco catalyst 3560 и IP телефонов Cisco 7960.

## Ход работы:
   В процессе выполнения лабораторной работы были выпонены следующие шаги:
   
   Построена топология сети, которая включает компьютеры, коммутаторы и роутер.
   
<img src="https://user-images.githubusercontent.com/58363643/226111767-13fcd8f0-4ae9-45b7-9f0d-ce620fa445f0.png" width="400">

  В конфигурационном режиме изменено название маршрутизатора на CMERouter.<br/>
  Отключty синтаксис ввода слов от DNS серверов с помощью команды:
  
    no ip domain-lookup 
    
  Заданы пароли для защиты маршрутизатора как в удаленном режиме, так и в режиме консоли.
  
  <img src="https://user-images.githubusercontent.com/58363643/226111876-2e98ef9b-1d33-4b35-a9b4-71de7e35d273.png" width="300">
  
  Настроен интерфейс fa0/0 на маршрутизаторе Cisco 2811 (CMERouter).

<img src="https://user-images.githubusercontent.com/58363643/226110660-4c0bd2d8-dc6e-4360-84ab-d5d4ba4e46d6.png" width="500">

  Настроен DHCP сервер для передачи голоса и данных на маршрутизаторе Cisco 2811.
  Настроены услуги телефонии Cisco CallManager Express на маршрутизаторе 2811.
  
  <img src="https://user-images.githubusercontent.com/58363643/226110760-1848636d-4066-4f96-b4d1-c6d36c9e577a.png" width="500">
  <img src="https://user-images.githubusercontent.com/58363643/226110963-ac032ecb-2eb1-4d25-b142-7a37ff90a92d.png" width="500">
  
  Созданы VLAN порты на коммутаторе Cisco Catalyst 3560 для взаимодействия коммутатора с маршрутизатором и подключены IP телефоны. Настроены IP-телефоны и соединены с коммутатором Cisco Catalyst 3560.

  <img src="https://user-images.githubusercontent.com/58363643/226111051-fa558b74-6938-4e65-a42f-de6a004c9606.png" width="300">
    <img src="https://user-images.githubusercontent.com/58363643/226111163-67bb291a-5a50-4aab-a0a8-182e8c9be021.png" width="500">

Проверены звонки между телефонами.

<img src="https://user-images.githubusercontent.com/58363643/226111592-be6208b4-a036-4423-818b-3ec6a4d518f2.png" width="500">

Созданы VLAN порты на коммутаторе для взаимодействия коммутатора с маршрутизатором и подключены IP телефоны.

<img src="https://user-images.githubusercontent.com/58363643/226112168-19b2d981-4f2b-4a2a-8872-066dd844beb0.png" width="500">
![image](https://user-images.githubusercontent.com/58363643/226112832-49a38080-74d2-4382-9445-3e813b6b65f8.png)

Задан маршрут по умолчанию командой 

    ip default-gateway.
    
Настроен порт как канал типа trunk.

![image](https://user-images.githubusercontent.com/58363643/226112598-75ce35b5-f08c-4c6b-8f40-a748ca83aabf.png)
![image](https://user-images.githubusercontent.com/58363643/226112675-8ec3e3ec-cfd8-4964-8c74-7450456f4d0f.png)

Настроен DHCP сервер для передачи голоса и данных на маршрутизаторе Cisco 2811.
Настроены услуги телефонии Cisco CallManager Express на маршрутизаторе.
Настроены IP-телефоны и соединены с коммутатором.
Подключены конечные узлы устройств.

![image](https://user-images.githubusercontent.com/58363643/226112906-b977ef34-fcde-4bee-998c-33581fd1fada.png)
![image](https://user-images.githubusercontent.com/58363643/226112948-3a83d206-fb2b-4e05-a39b-703e1d18853e.png)

<img src="https://user-images.githubusercontent.com/58363643/226121120-9b091b54-1d92-44fc-bc56-c0fe8089467e.png" width="400">

Проверить звонки между телефонами

<img src="https://user-images.githubusercontent.com/58363643/226121168-eead5dc4-1a2b-4818-8ab7-a731ca25aad1.png" width="400">

![image](https://user-images.githubusercontent.com/58363643/226122219-9d833d2e-6389-4a9a-9af6-c28df6e6cecf.png)

## Выводы:
Таким образом, была изучена схема настройки IP-телефонии с помощью CallManager Express.
