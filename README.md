# OM-DZ04

На виртуальной машине установлена CMS wordpress, которая включает в себя следующие компоненты:

nginx, php-fpm, database (MySQL)

На CMS развернут тестовый домен http://www.example.com/

---

Ранне был развернут сервер Prometheus с помощью docker-compose. 

Добавляем в docker-compose.yml конфигурацию для запуска сервера Grafana.

Запускаем сервисы.

docker-compose up -d

Подключаемся к Grafana по адресу http://localhost:3000/

Настраиваем в качестве источника данных Prometheus:

![s5](https://github.com/user-attachments/assets/b896b0b3-78e5-4ebd-bc88-abde42691bb3)

---

Создаем внутри Grafana папки с названиями infra и app.

![s1](https://github.com/user-attachments/assets/524270b8-6d98-473c-a001-76f846ea4eef)

![s2](https://github.com/user-attachments/assets/dc2676f2-6bc8-4ad0-9e12-b6ccc4c94d58)

---




