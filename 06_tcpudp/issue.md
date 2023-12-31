# Не работает telnet ни на стороне Kali, ни на стороне Ubuntu
Не работает если указать IP другой машины или IP и порт

## При пинговании ситуация следующая:
На стороне Kali:
![image](https://github.com/VladKoretski/ibnet-homeworks/assets/130839671/1fa85274-f826-49c8-8e80-facd85fe1853)
На стороне Ubuntu:
![image](https://github.com/VladKoretski/ibnet-homeworks/assets/130839671/e261592c-18e4-4473-9f6a-41ff9d952869)

То есть, связь есть между Ubuntu и Kali! - такой вывод.

## На Kali выполняю следующие команды:
1. sudo apt update
2. sudo apt install telnet
## На Ubuntu выволняю следующие команды:
sudo apt update
sudo apt install nginx openssh-server vsftpd telnet

После запусках telnet на обоих машинах получаю сообщение 
telnet: Unable to connect to remote host: Connection refused:

На Ubuntu
![image](https://github.com/VladKoretski/ibnet-homeworks/assets/130839671/8f86a7c8-5193-404e-bcf3-862794200c0b)

На Kali
![image](https://github.com/VladKoretski/ibnet-homeworks/assets/130839671/8aed5272-ee1e-49b5-8ddb-e3835f7d6d1a)

Аналогичная ситуация, если я использую адреса из описания домашней работы: Ubuntu - 192.168.0.1, Kali - 192.168.0.2

## У меня следующие сетевые настройки:
### На Kali:
![image](https://github.com/VladKoretski/ibnet-homeworks/assets/130839671/d9b801a9-39c2-458e-8b79-86002cc3142f)
![image](https://github.com/VladKoretski/ibnet-homeworks/assets/130839671/0977c7e3-a96e-4b80-a37b-f1b8697f927f)


### На Ubuntu
![image](https://github.com/VladKoretski/ibnet-homeworks/assets/130839671/5a3e5285-7ada-408f-8cab-ed317482faf2)
![image](https://github.com/VladKoretski/ibnet-homeworks/assets/130839671/383aea08-864c-44d2-9634-19a89c342073)

Есть еще такой момент: ошибка при установке telnet на Ubuntu:
![image](https://github.com/VladKoretski/ibnet-homeworks/assets/130839671/04703bfe-a6c5-4dfa-a4b8-62aeb4f22420)



