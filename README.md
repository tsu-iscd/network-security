# Основы построения защищенных компьютерных сетей

## Описание курса

Программа и материалы курса «Основы построения защищенных компьютерных сетей»
образовательной программы по направлению подготовки (специальности)
10.05.01 «Компьютерная безопасность», преподаваемого в [Национальном исследовательском Томском государственном университете](http://www.tsu.ru) на [кафедре защиты информации и киптографии](http://isc.tsu.ru)

## Вопросы

1. Сетевые атаки
    * ARP spoofing
    * MAC spoofing
    * IP-spoofing
    * TCP-hijacking
    * DHCP-spoofing
2. DOS- и DDoS- атаки
    * Классические DoS-атаки
      * Ping of Death
      * SMURF
      * LAND
    * NTP amplification
    * DNS amplification
    * DoS-атаки на протокол HTTP
3. Межсетевое экранирование
    * Виды межсетевых экранов
    * Архитектура межсетевых экранов
    * Режимы работы
      * routed
      * transparent
    * Межсетевые экраны с инспекцией состояний
    * Технологии NAT, Identity Firewall, PVLAN
    * Основные схемы подлючения
    * Конфигурация межсетевых экранов
4. Технология IPSec VPN
    * Технология VPN
    * Классификация VPN
    * Протоколы AH, ESP, IKE
    * Режимы работы IPSec
    * Основные схемы организации VPN
    * GRE over IPSec и IPSec over GRE
5. Системы обнаружения вторжений
    * Виды СОВ
    * Проблема ложных срабатываний
    * Модель CIDF 
    * Методы обнаружения вторжений
    * Основные схемы подключения СОВ
    * Методы повышения точности настройки СОВ и управления сигнатурами
    * Механизмы повышения отказоустойчивости
6. Платформы сетевых средств защиты
    * Программные
    * Программно-аппаратные
    * Виртуальные 
    * Шассийные
    * Интегрируемые
    * Best practices
7. Защита сетевых устройств 
8. Дизайн защищенных сетей
    * Дизайн ЛВС
    * Дизайн ГВС
    * Дизайн периметра Интернет
    * Управление сетевыми потоками сетевых служб (DNS, SMTP, WEB)
9. Протоколы SSL/TLS
    * Основные механизмы протоколов
    * PKI
    * Конфигурация SSL/TLS
    * Атаки на SSL/TLS
    
## Лабораторные работы

1. Настройка Cisco IOS
2. Защита инфраструктуры маршрутизации
3. Защита инфраструктуры коммутации
4. Построение отказоустойчивой ЛВС на базе протокола STP
5. Защита ЛВС от атак канального уровня
6. Построение маршрутизируемой ЛВС
7. Защита сетевой инфраструктуры от НСД
8. Защита периметра сети
9. Криптографическая защита каналов передачи данных от несанкционированного доступа
10. Защита беспроводной ЛВС

## Дополнительные задания
1. Сгенерировать цепочку сертификатов (корневой, промежуточный, клиента, сервреа и т.д.). Настроить аутентификацию клиента перед веб-сервером по сертификату.
2. На защищаемом сервере установить и настроить систему обнаружения и предотвращения атак [Snort](https://www.snort.org/). Написать следующие правила Snort, реализующие:
      * обнаружение взаимодействия зараженных браузеров с сервером BeEF
      * обнаружение атаки Heartbleed
      * обнаружение атаки SSRF
3. На основе фрэймворка GNS3 реализовать динамическую маршрутизацию по протоколу OSPF по схеме [Point-to-Point GRE over IPSec] (http://www.cisco.com/c/en/us/td/docs/solutions/Enterprise/WAN_and_MAN/P2P_GRE_IPSec/P2P_GRE/2_p2pGRE_Phase2.html). Тестовое окружение состоит из трех маршрутизаторов, соединение которых представляет топологию звезда (Hub-and-Spoke). На всех маршрутизаторах выполнить [настройку механизмов защиты от несанкционированного доступа] (http://www.cisco.com/c/en/us/td/docs/solutions/Enterprise/Security/Baseline_Security/securebasebook/sec_chap2.html). 
4. Проанализировать конфигурационный файл и ответить на вопрос: можно ли используя учетную запись `cisco` паролем `cisco`
зайти на устройство с такими настройками, если на AAA сервере TMK2 создана учетная запись cisco с паролем cisco.

## Материалы

### Литература
* [Sean Convery. Network Security Architectures](http://www.amazon.com/Network-Security-Architectures-Networking-Technology/dp/158714297X)
* [Cisco Network Security Baseline](http://www.cisco.com/c/en/us/td/docs/solutions/Enterprise/Security/Baseline_Security/securebasebook.html)
* [Ivan Ristić. Bulletproof SSL and TLS](https://www.feistyduck.com/books/bulletproof-ssl-and-tls/)
* [Eric Vyncke. LAN Switch Security: What Hackers Know About Your Switches](http://www.amazon.com/LAN-Switch-Security-Hackers-Switches/dp/1587052563)

### Справочная литература
* [Cisco SAFE reference Guide](http://www.cisco.com/c/en/us/td/docs/solutions/Enterprise/Security/SAFE_RG/SAFE_rg.html)
* [TCP/IP Illustrated. Volume 1: The Protocols (2nd Edition)](http://www.amazon.com/gp/product/0321336313/)
* 
### Курсы
* [Спецкурсы лаборатории безопасности информационных систем ВМК МГУ](http://course.secsem.ru/lections)
