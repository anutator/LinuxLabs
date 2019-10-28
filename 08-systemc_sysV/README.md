## Разворачиваем JIRA Atlassian в Vagrant и заменяем init на unit

#### Немного информации:
В unit  файле сервиса я использовал тип forking, так как информация, которая у меня есть, гласит о том, что для Tomcat, Java лучше подходит использование Type=forking

### Как запустить проект:
1. Версия vagrant 2.2.4 должна быть, почему-то у меня на 2.2.5 не запустился проект.
2. Скачать весь репозиторий и перейти в каталог lab-7, и в нем запустить  vagran up
3. Скачать Vagrantfile + jira_deploy.sh в свой какой угодно каталог, в каталоге  выполнить потом  vagrant init после этого запускаем vagrant up
4. По завершении деплоя вы увидите:
```
jiraserver: JIRA Atlassian installed and running!
```
что гласит о том, что все хорошо и Jira Atlassian готов вам принять на 
```
http://10.10.10.20:8070/
```
в случае если будет все плохо будут сообщения с ошибками, которые надо будет фиксить. Скорее всего вы изменили исходные скрипты и поэтому что-то пошло не так.

```
 все скачанные скрипты можете изменять как вам угодно,  если не будет работать, я не виноват =)
```