# OM-DZ04

На виртуальной машине установлена CMS wordpress, которая включает в себя следующие компоненты:

nginx, php-fpm, database (MySQL)

На CMS развернут тестовый домен http://www.example.com/

---

Раннее был развернут сервер Prometheus с помощью docker-compose. 

Добавляем в docker-compose.yml конфигурацию для запуска сервера Grafana.

Запускаем сервисы.

docker-compose up -d

Подключаемся к Grafana по адресу http://localhost:3000/

Настраиваем в качестве источника данных Prometheus:

![s5](https://github.com/user-attachments/assets/b896b0b3-78e5-4ebd-bc88-abde42691bb3)

---

Создаем внутри Grafana папки с названиями infra и app.

![s2](https://github.com/user-attachments/assets/5d72c141-c4d3-4a5c-96c1-812fddeb151f)

![s1](https://github.com/user-attachments/assets/0f454952-e2bd-45ba-bdda-a21490af0cf0)

---

Внутри директории infra создаем дашборд, для отображения сводной информации 
по инфраструктуре (CPU, RAM, Network, etc.)

![s3](https://github.com/user-attachments/assets/7358bd2d-d98f-43c8-bfc0-1c8edf4e1caa)

---

Внутри директории app создаем дашборд, для отображения сводной информации 
о CMS (доступность компонентов, время ответа, etc.)

![s4](https://github.com/user-attachments/assets/33251b84-9211-4102-9661-ec2518f4dba4)

