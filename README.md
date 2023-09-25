# Задание 1
Создайте собственный образ любой операционной системы (например, debian-11) с помощью Packer (инструкция для установки плагина yandex-cloud).

Чтобы получить зачёт, вам нужно предоставить скриншот страницы с созданным образом из личного кабинета YandexCloud.
# Решение
![image](https://github.com/Kul-RB/devops-netology/assets/53901269/9a787132-6707-4233-b39a-7bef0e2fef1f)

# Задание 2.1
Создайте вашу первую виртуальную машину в YandexCloud с помощью web-интерфейса YandexCloud.
# Решение
![image](https://github.com/Kul-RB/devops-netology/assets/53901269/1b76c347-129c-4491-8f1b-78a3c941185e)
![image](https://github.com/Kul-RB/devops-netology/assets/53901269/d6470f1e-3748-4c1d-b3b6-ac237244dc2d)

# Задание 2.2
Создайте вашу первую виртуальную машину в YandexCloud с помощью Terraform (вместо использования веб-интерфейса YandexCloud). Используйте Terraform-код в директории (src/terraform).
# Решение
![image](https://github.com/Kul-RB/devops-netology/assets/53901269/54669c75-a43c-4c94-91c7-36222fb11608)
![image](https://github.com/Kul-RB/devops-netology/assets/53901269/af10e7df-0bbb-470b-86f3-dfd1fdc815c9)

# Задание 3
С помощью Ansible и Docker Compose разверните на виртуальной машине из предыдущего задания систему мониторинга на основе Prometheus/Grafana. Используйте Ansible-код в директории (src/ansible).

Чтобы получить зачёт, вам нужно предоставить вывод команды "docker ps" , все контейнеры, описанные в docker-compose, должны быть в статусе "Up".
# Решение
![image](https://github.com/Kul-RB/devops-netology/assets/53901269/f679904c-71e7-4461-a306-44c1f9a5ca83)

# Задание 4 
Откройте веб-браузер, зайдите на страницу http://<внешний_ip_адрес_вашей_ВМ>:3000.
Используйте для авторизации логин и пароль из .env-file.
Изучите доступный интерфейс, найдите в интерфейсе автоматически созданные docker-compose-панели с графиками(dashboards).
Подождите 5-10 минут, чтобы система мониторинга успела накопить данные.
# Решение
![image](https://github.com/Kul-RB/devops-netology/assets/53901269/5a3f2b24-0076-4b4d-a1fc-e0000cf7ede1)

# Задание 5
Создайте вторую ВМ и подключите её к мониторингу, развёрнутому на первом сервере.

Чтобы получить зачёт, предоставьте:

скриншот из Grafana, на котором будут отображаться метрики добавленного вами сервера.

# Решение
![image](https://github.com/Kul-RB/devops-netology/assets/53901269/defda151-b522-4701-95f4-32ccb4c232ce)



