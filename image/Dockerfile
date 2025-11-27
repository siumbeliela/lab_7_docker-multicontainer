# Используем минимальный образ, например, Alpine
FROM alpine:latest

# Копируем изображение в контейнер
COPY my_image.jpg /usr/share/image/my_image.jpg

# Устанавливаем простой сервер для показа файла (опционально)
RUN apk add --no-cache python3 py3-pip
CMD ["python3", "-m", "http.server", "8080", "--directory", "/usr/share/image"]

# Открываем порт 8080
EXPOSE 8080
