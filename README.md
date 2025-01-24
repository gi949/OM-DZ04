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

