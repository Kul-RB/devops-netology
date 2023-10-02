# ls
Чек-лист готовности к домашнему заданию
Скачайте и установите актуальную версию Terraform >=1.4.X . Приложите скриншот вывода команды terraform --version.
Скачайте на свой ПК этот git-репозиторий. Исходный код для выполнения задания расположен в директории 01/src.
Убедитесь, что в вашей ОС установлен docker.
Зарегистрируйте аккаунт на сайте https://hub.docker.com/, выполните команду docker login и введите логин, пароль

![image](https://github.com/Kul-RB/devops-netology/assets/53901269/ead61809-f7e8-4474-85a1-e5387eb8a7ec)
![image](https://github.com/Kul-RB/devops-netology/assets/53901269/2d239238-cf6b-43e6-bc74-9667a6e85dde)
![image](https://github.com/Kul-RB/devops-netology/assets/53901269/06892f4f-b04e-4a13-b4c3-776141d43849)
![image](https://github.com/Kul-RB/devops-netology/assets/53901269/5f4b5143-0308-448d-a496-6700ca4d3387)

# Задание 1
1. Перейдите в каталог src. Скачайте все необходимые зависимости, использованные в проекте.
2. Изучите файл .gitignore. В каком terraform-файле, согласно этому .gitignore, допустимо сохранить личную, секретную информацию?
3. Выполните код проекта. Найдите в state-файле секретное содержимое созданного ресурса random_password, пришлите в качестве ответа конкретный ключ и его значение.
4. Раскомментируйте блок кода, примерно расположенный на строчках 29–42 файла main.tf. Выполните команду terraform validate. Объясните, в чём заключаются намеренно допущенные ошибки. Исправьте их.
5. Выполните код. В качестве ответа приложите: исправленный фрагмент кода и вывод команды docker ps.
6. Замените имя docker-контейнера в блоке кода на hello_world. Не перепутайте имя контейнера и имя образа. Мы всё ещё продолжаем использовать name = "nginx:latest". Выполните команду terraform apply -auto-approve.
7. Объясните своими словами, в чём может быть опасность применения ключа -auto-approve. В качестве ответа дополнительно приложите вывод команды docker ps.
8. Уничтожьте созданные ресурсы с помощью terraform. Убедитесь, что все ресурсы удалены. Приложите содержимое файла terraform.tfstate.
9. Объясните, почему при этом не был удалён docker-образ nginx:latest. Ответ обязательно подкрепите строчкой из документации terraform провайдера docker. (ищите в классификаторе resource docker_image )

# Решение
1. ![image](https://github.com/Kul-RB/devops-netology/assets/53901269/0e3d2a64-6cdd-44b6-94f0-5e0dbc7901ee)

2. Согласно .gitignore хранение серкретной информации осуществляется в файле personal.auto.tfvars
3. ![image](https://github.com/Kul-RB/devops-netology/assets/53901269/b71e43be-6839-4dfa-b0dd-ad6515f17f92)

4.1 ![image](https://github.com/Kul-RB/devops-netology/assets/53901269/964f315d-107b-4e02-8aa7-eb4ec81c4fa4)
Пропущено имя ресурса, блок resource должен состоять из типа и имени
4.2 ![image](https://github.com/Kul-RB/devops-netology/assets/53901269/27a36d5e-5992-4e98-be15-1ba57b974f3f)
Неправильное наименование ресурса, наименвоание должно начинаться с буквы или подчеркивания и может содержать только буквы, цифры, подчеркивания и тире
4.3 ![image](https://github.com/Kul-RB/devops-netology/assets/53901269/e04f842d-a345-47ce-8279-c627bc03cf26)
random_string_FAKE не объявлен в "random_password"
4.4 ![image](https://github.com/Kul-RB/devops-netology/assets/53901269/68a0ce6b-de27-4b6a-bca0-b7466c42db09)
Неправильное наименование атрибута result, вместо resulT необходимо написать result
