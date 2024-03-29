# Домашнее задание к занятию 4. «Оркестрация группой Docker-контейнеров на примере Docker Compose»


## Задача 1

Создайте собственный образ любой операционной системы (например ubuntu-20.04) с помощью Packer ([инструкция](https://cloud.yandex.ru/docs/tutorials/infrastructure-management/packer-quickstart)).

Чтобы получить зачёт, вам нужно предоставить скриншот страницы с созданным образом из личного кабинета YandexCloud.

### Ответ

![Скрин](https://github.com/Jlljully/Virtualization/blob/main/files/lesson_4/Screenshot_1.png "пакер")

![Скрин](https://github.com/Jlljully/Virtualization/blob/main/files/lesson_4/Screenshot_2.png "пакер")

Переделала на центос

![Скрин](https://github.com/Jlljully/Virtualization/blob/main/files/lesson_4/Untitled14.png "пакер") 


## Задача 2

**2.1.** Создайте вашу первую виртуальную машину в YandexCloud с помощью web-интерфейса YandexCloud.        

**2.2.*** **(Необязательное задание)**      
Создайте вашу первую виртуальную машину в YandexCloud с помощью Terraform (вместо использования веб-интерфейса YandexCloud).
Используйте Terraform-код в директории ([src/terraform](https://github.com/netology-group/virt-homeworks/tree/virt-11/05-virt-04-docker-compose/src/terraform)).

Чтобы получить зачёт, вам нужно предоставить вывод команды terraform apply и страницы свойств, созданной ВМ из личного кабинета YandexCloud.

### Ответ

Созданная вручную:  

![Скрин](https://github.com/Jlljully/Virtualization/blob/main/files/lesson_4/Untitled8.png "вм")  

Созданная терраформом:  

![Скрин](https://github.com/Jlljully/Virtualization/blob/main/files/lesson_4/Untitled9.png "вм") 

![Скрин](https://github.com/Jlljully/Virtualization/blob/main/files/lesson_4/Untitled10.png "вм") 

## Задача 3

С помощью Ansible и Docker Compose разверните на виртуальной машине из предыдущего задания систему мониторинга на основе Prometheus/Grafana.
Используйте Ansible-код в директории ([src/ansible](https://github.com/netology-group/virt-homeworks/tree/virt-11/05-virt-04-docker-compose/src/ansible)).

Чтобы получить зачёт, вам нужно предоставить вывод команды "docker ps" , все контейнеры, описанные в [docker-compose](https://github.com/netology-group/virt-homeworks/blob/virt-11/05-virt-04-docker-compose/src/ansible/stack/docker-compose.yaml),  должны быть в статусе "Up".

### Ответ

![Скрин](https://github.com/Jlljully/Virtualization/blob/main/files/lesson_4/Untitled11.png "ansible") 

![Скрин](https://github.com/Jlljully/Virtualization/blob/main/files/lesson_4/Untitled12.png "ansible") 


## Задача 4

1. Откройте веб-браузер, зайдите на страницу http://<внешний_ip_адрес_вашей_ВМ>:3000.
2. Используйте для авторизации логин и пароль из [.env-file](https://github.com/netology-group/virt-homeworks/blob/virt-11/05-virt-04-docker-compose/src/ansible/stack/.env).
3. Изучите доступный интерфейс, найдите в интерфейсе автоматически созданные docker-compose-панели с графиками([dashboards](https://grafana.com/docs/grafana/latest/dashboards/use-dashboards/)).
4. Подождите 5-10 минут, чтобы система мониторинга успела накопить данные.

Чтобы получить зачёт, предоставьте: 

- скриншот работающего веб-интерфейса Grafana с текущими метриками, как на примере ниже.


### Ответ

![Скрин](https://github.com/Jlljully/Virtualization/blob/main/files/lesson_4/Untitled13.png "графана") 

## Задача 5 (*)

Создайте вторую ВМ и подключите её к мониторингу, развёрнутому на первом сервере.

Чтобы получить зачёт, предоставьте:

- скриншот из Grafana, на котором будут отображаться метрики добавленного вами сервера.


### Ответ
