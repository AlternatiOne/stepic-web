## Вспомогательный репозиторий для курса [Web-технологии](https://stepik.org/course/154)

### [Задание](https://stepik.org/lesson/14825/step/12?unit=4174)

#### Отдача статических файлов
1) Установите Web-сервер nginx

2) В директории `/home/box` (домашняя директория) создайте следующую структуру директорий:

```
/home/box/web
          |---public
          |   |---img
          |   |---css
          |   |---js
          |---uploads
          |---etc
```
3) Настройте nginx так, чтобы:
   - Все URL, начинающиеся с `/uploads/` (например, `/uploads/1.jpeg`) отдавались из директории `/home/box/web/uploads`
   - Все URL с расширением (например, `/img/1.jpeg`) отдавались из директории `/home/box/web/public`
   - Все URL без расширения (например, `/question/123`) возвращали HTTP 404
  
4) Фрагмент конфига nginx, который обслуживает ваш проект, должен находиться в файле `/home/box/web/etc/nginx.conf` и должен быть включен в основной конфиг с помощью символической ссылки.

5) Запустите nginx так, чтобы он принимал запросы на порту 80 и обслуживал бы любые домены.

6) Не забудьте закоммитить и сохранить на Github полученную структуру директорий и конфиги.

---
### Дата создания репозитория
2016.05.16
