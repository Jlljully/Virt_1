
# Домашнее задание к занятию 2. «Применение принципов IaaC в работе с виртуальными машинами»


## Задача 1

- Опишите основные преимущества применения на практике IaaC-паттернов.
- Какой из принципов IaaC является основополагающим?

### Ответ

Ускоряет процесс предоставления инфраструктуры по мере необходимости  
Позволяет устранить "дрейф конфигурации", когда среды разработки и тестирования не совдпадают  
Ускоряет каждый этап жизни ПО из-за скорости развертывания тестовых сред  
Автодокументирование всей инфраструктуры из того же кода   
  
Идемпотентность - всегда предсказуемый результат  

## Задача 2

- Чем Ansible выгодно отличается от других систем управление конфигурациями?
- Какой, на ваш взгляд, метод работы систем конфигурации более надёжный — push или pull?

### Ответ

Низкий порог входа при обучении. Написан на python, который учил, как мне кажется, каждый в IT в той или иной мере.   
  
Push  - конфигурация отправляется центральным управляющим сервером на целевые хосты, то есть инициализация применения изменений централизованная, что гарантирует единообразие всех подключенных систем. К тому же, его использует Ansible - самая популярная сейчас система управления конфигурациями, то есть профессионалы повсеместно отдают предпочтение именно push режиму.


## Задача 3

Установите на личный компьютер:

- [VirtualBox](https://www.virtualbox.org/),
- [Vagrant](https://github.com/netology-code/devops-materials),
- [Terraform](https://github.com/netology-code/devops-materials/blob/master/README.md),
- Ansible.

*Приложите вывод команд установленных версий каждой из программ, оформленный в Markdown.*

### Ответ

![Скрин](https://github.com/Jlljully/Virtualization/blob/main/files/lesson_2/Screenshot_1.png "1")  
  
![Скрин](https://github.com/Jlljully/Virtualization/blob/main/files/lesson_2/Screenshot_2.png "2")  

![Скрин](https://github.com/Jlljully/Virtualization/blob/main/files/lesson_2/Screenshot_3.png "3")  

## Задача 4 

Воспроизведите практическую часть лекции самостоятельно.

- Создайте виртуальную машину.
- Зайдите внутрь ВМ, убедитесь, что Docker установлен с помощью команды
```
docker ps,
```
Vagrantfile из лекции и код ansible находятся в [папке](https://github.com/netology-code/virt-homeworks/tree/virt-11/05-virt-02-iaac/src).

Примечание. Если Vagrant выдаёт ошибку:
```
URL: ["https://vagrantcloud.com/bento/ubuntu-20.04"]     
Error: The requested URL returned error: 404:
```

выполните следующие действия:

1. Скачайте с [сайта](https://app.vagrantup.com/bento/boxes/ubuntu-20.04) файл-образ "bento/ubuntu-20.04".
2. Добавьте его в список образов Vagrant: "vagrant box add bento/ubuntu-20.04 <путь к файлу>".


### Ответ

![Скрин](https://github.com/Jlljully/Virtualization/blob/main/files/lesson_2/Screenshot_4.png "4")  

![Скрин](https://github.com/Jlljully/Virtualization/blob/main/files/lesson_2/Screenshot_5.png "5")  

Вторую часть пришлось выполнять на виртуалбоксе на убунте, поднятой на виртуалбоксе на виндоус из-за неработающего на виндоус ансибла:  

![Скрин](https://github.com/Jlljully/Virtualization/blob/main/files/lesson_2/Screenshot_7.png "5")
