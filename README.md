# Ansible_tutorial
<p style="text-align: center;">My homework by Ansible</p>

## Создание ssh-соединения между клиентом и сервером
### Генерируем ssh-ключ на клиенте
    ssh-keygen -t ed25519 -C "ansible"

### Копируем открытый ssh-ключ на удаленный сервер
    ssh-copy-id -i ~/.ssh/ansible.pub -p 2022 adalbera@10.0.2.15

    По умолчанию ssh-сервер прослушивает на удаленном сервере 22 порт.

### Проверяем список установленных ключей на удаленном сервере
    cat /.ssh/authorized_keys

### Подключаемся к удаленному серверу
    ssh -i ~/.ssh/ansible -p 2022 adalbera@10.0.2.15



  