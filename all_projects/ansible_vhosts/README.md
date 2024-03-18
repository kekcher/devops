Создание трёх виртуальных хостов при помощи ansible
===

### Порядок выполнения работы
- Создаём папку ansible_vhosts
* mkdir ansible_vhosts
- Наполняем эту папку файлами
* > inventory.ini(здесь хранится ip машины)
* > playbook.yml(здесь хранится имя роли и три сайта, которые будут запускаться)
* > run_playbook.sh(здесь хранится скрипт shell, который запускает playbook с запросом пароля)
- Создаём папку с ролями role/nginx-vhosts
- В папке nginx-vhosts создаём папку handlers
* > В папке handlers находится обработчик main.yml, который отвечает за рестарт nginx
- В папке nginx-vhosts создаём папку tasks
* > В папке tasks находится обработчик main.yml, который отвечает за формирование сайтов в цикле
- В папке nginx-vhosts создаём папку templates
* > В папке templates прописываем выводимый html index.html.j2 и конфиг для сервера site.conf.j2
- Запускаем наш срипт shell(sh run_playbook.sh)
