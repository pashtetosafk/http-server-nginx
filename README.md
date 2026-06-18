# HTTP Server with Nginx Reverse Proxy

## Технологии
- Docker / Docker Compose
- Nginx (reverse proxy)
- Python 3.9 (HTTP server)

## Быстрый старт

### 1. Клонирование репозитория

```bash
git clone https://github.com/pashtetosafk/http-server-nginx.git
cd http-server-nginx
```
### 2. Запуск проекта

```bash
docker-compose up -d --build
```
### 3. Проверка работы
```bash
curl http://localhost/
```
### 4. Остановка
```bash
docker-compose down
```
## Как работает
#### 1. Nginx (порт 80) принимает запросы снаружи
#### 2. Проксирует их на Backend (порт 8080) по имени сервиса backend
#### 3. Backend (Python) обрабатывает запрос и возвращает ответ
