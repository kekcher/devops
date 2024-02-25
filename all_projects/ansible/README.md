Ansible-playbook
===

### Порядок выполнения работы
- В настройках Виртуальной машины, в разделе сеть ставим виртуальный адаптер и NAT
- У нас сгенерирован ключ, который располагается по пути .ssh/authorized_keys
- Скачаиваем ansible (sudo apt install ansible)
- Создаём директорию ansible_dir и вносим туда необходимые файлы
* mkdir ansible_dir
* cd ansible_dir
* > index.html
* > playbook.yml
- Редактриуем скрипты в index.html и playbook.yml
- Запускаем скрипт (sudo ansible-playbook playbook.yml)
- Вводим в поисковик localhost и открывается разметка, которая прописана в index.html
