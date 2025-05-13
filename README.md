# ansible
1. Запуск playbook на окружении из test.yml

![alt text](<Screenshot 2025-05-06 165053.jpg>)

2. Изменение значения some_fact

![alt text](<Screenshot 2025-05-06 170154.jpg>)

4. Запуск prod.yml

![alt text](<Screenshot 2025-05-12 175145.jpg>)

5. Добавьте факты в group_vars

![alt text](<Screenshot 2025-05-12 175420.jpg>)

7. При помощи ansible-vault зашифруйте факты

![alt text](<Screenshot 2025-05-12 175719.jpg>)

8. Запустите playbook на окружении prod.yml. При запуске ansible должен запросить у вас пароль. Убедитесь в работоспособности.

![alt text](<Screenshot 2025-05-12 175859.jpg>) 

9. Выбор плагина для control node

ansible-doc -t connection -l

Выбрается плагин local

10. Добавление группы local

local:
    hosts:
      localhost:
        ansible_connection: local

11. Финальный запуск playbook

![alt text](<Screenshot 2025-05-13 103921.jpg>)
