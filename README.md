# Hi, This is test repository for ansible stokly

#### Описание Ролей:     
add_user - добавление пользователя с генерацией пароля и ssh ключем
delete_user - удаление пользователей
delete_pkg - удаление пакетов

#### Запуск роли:    
ansible-playbook -i inventory all.yml --ask-vault-pass     

#### Запуск под пользователем из группы sudo      
ansible-playbook -i inventory all.yml --ask-vault-pass --ask-become-pass

#### Работа с vault  
ansible-vault decrypt group_vars/all/vault.yml - Расшифровать файл переменных   
ansible-vault encrypt group_vars/all/vault.yml - Зашифровать файл переменных