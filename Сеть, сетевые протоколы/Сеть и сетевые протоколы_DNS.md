# Домашнее задание к занятию "`Сеть и сетевые протоколы: DNS`" - `Семенов С.В.`


### Задание 1. 

Может ли компьютер работать без `DNS`? Будет ли работать сеть если в ней нет `DNS-сервера`? 

*Приведите ответ в свободной форме.*

### Ответ.
Компьютер без проблем может работать без DNS. Тем более, если он не подключен ни к локальной сети, ни к глобальной сети Интернет. Кроме этого, сеть тоже может работать без DNS-сервера. В этом случае обращаться к хостам придется по IP-адресам. Это касается всех сетей, так как основная задача DNS найти числовой идентификатор по понятному для человека имени.

---

### Задание 2. 

Кто выдает DNS имена? 

*Приведите ответ в свободной форме.*

### Ответ.
На сегодня ICANN использует распределённую систему регистрации доменов, которая основана на принципе свободного доступа аккредитованных регистраторов к реестрам доменных имен. В России администратором реестра доменных имен является Координационный центр национального домена сети Интернет. Эта организация регулирует работу регистраторов в России. DNS-имя или домен можно зарегистрировать в любом аккредитованном регистраторе.


---

### Задание 3. 

Где в Linux настраивается DNS-клиент в простейшем случае?

*Приведите ответ в свободной форме.*

### Ответ.
В простейшем случае DNS-клиент в Linux настраивается в через файл /etc/hosts, который работает в качестве базы данных имен и адресов. Синтаксис /etc/hosts предельно простой: IP адрес, полное имя (FQDN) набор алиасов (дополнительных имен).
Кроме этого, DNS-клиент настраивается в файлах конфигурации /etc/resolv.conf и /etc/nsswitch.conf. В первом настраивается список DNS-серверов, во-втором, список модулей, к которым обращается система при резолве имен. К примеру, могут быть указаны модули `files` `dns` `hostname`. 

---

### Задание 4. 

Для чего служит ресурсная DNS запись типа `MX`?

*Приведите ответ в свободной форме.*

### Ответ.
Ресурсная DNS запись типа `MX` служит для указания почтового шлюза для домена. Состоит из двух частей: приоритета (чем число больше, тем ниже приоритет) и адреса узла.


---


