# Домашнее задание "Основы сбора и хранения логов"


Задание выполнялось по инструкии из методички с отправкой логов через rsyslog.

Установка и проверка nginx на VM web:

![Image alt](https://github.com/AlexndrVakulenko/homework17/blob/main/01_%D0%9F%D1%80%D0%BE%D0%B2%D0%B5%D1%80%D0%BA%D0%B0_service_nginx.png)

![Image alt](https://github.com/AlexndrVakulenko/homework17/blob/main/02_%D0%A1%D1%82%D0%B0%D1%80%D1%82%D0%BE%D0%B2%D0%B0%D1%8F%D0%A1%D1%82%D1%80%D0%B0%D0%BD%D0%B8%D1%86%D0%B0_nginx.png)

Проверка установки rsyslog:

![Image alt](https://github.com/AlexndrVakulenko/homework17/blob/main/03_%D0%9F%D1%80%D0%BE%D0%B2%D0%B5%D1%80%D0%BA%D0%B0_rsyslog_date_%D0%BD%D0%B0_VM_log.png)

Редактирование /etc/rsyslog.conf

![Image alt](https://github.com/AlexndrVakulenko/homework17/blob/main/04_%D0%9A%D0%BE%D1%80%D1%80%D0%B5%D0%BA%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%BA%D0%B0_rsyslog.conf.png)

Перезапуск, проверка службы rsyslog

![Image alt](https://github.com/AlexndrVakulenko/homework17/blob/main/05_%D0%9F%D1%80%D0%BE%D0%B2%D0%B5%D1%80%D0%BA%D0%B0_rsyslog.service.png)

![Image alt](https://github.com/AlexndrVakulenko/homework17/blob/main/06_%D0%9F%D0%BE%D1%80%D1%82_514.png)

Настройка передачи логов nginx, проверка конфигурации nginx

![Image alt](https://github.com/AlexndrVakulenko/homework17/blob/main/07_%D0%9D%D0%B0%D1%81%D1%82%D1%80%D0%BE%D0%B9%D0%BA%D0%B0_%D0%BE%D1%82%D0%BF%D1%80%D0%B0%D0%B2%D0%BA%D0%B8_%D0%BB%D0%BE%D0%B3%D0%BE%D0%B2.png)

![Image alt](https://github.com/AlexndrVakulenko/homework17/blob/main/08_%D0%9F%D1%80%D0%BE%D0%B2%D0%B5%D1%80%D0%BA%D0%B0_%D0%BA%D0%BE%D0%BD%D1%84%D0%B8%D0%B3%D1%83%D1%80%D0%B0%D1%86%D0%B8%D0%B8_nginx.png)

Информация о логах на log-сервере

![Image alt](https://github.com/AlexndrVakulenko/homework17/blob/main/09_%D0%9F%D1%80%D0%BE%D0%B2%D0%B5%D1%80%D0%BA%D0%B0%D0%9E%D1%82%D0%BF%D1%80%D0%B0%D0%B2%D0%BA%D0%B8%D0%9B%D0%BE%D0%B3%D0%BE%D0%B2.png)

Симуляция ошибки перемещеним стартовой страницы: mv /var/www/html/index.nginx-debian.html /var/www/ 

![Image alt](https://github.com/AlexndrVakulenko/homework17/blob/main/10_%D0%9F%D1%80%D0%BE%D0%B2%D0%B5%D1%80%D0%BA%D0%B0%D0%9E%D1%82%D0%BF%D1%80%D0%B0%D0%B2%D0%BA%D0%B8%D0%9B%D0%BE%D0%B3%D0%BE%D0%B22.png)