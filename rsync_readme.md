Домашнее задание к занятию 3 «Резервное копирование»

Задание 1

Здесь мы создаем бэкап с помощью rsync, исключаем скрытые файлы и отслеживаем процесс выполнения программы. 

![Снимок экрана от 2024-03-11 09-48-26](https://github.com/Niko1a/lebedev/assets/110035244/e9d05053-4fef-4a3c-96fa-d596b8eb6496)

![Снимок экрана от 2024-03-11 09-49-51](https://github.com/Niko1a/lebedev/assets/110035244/451fcb66-006b-4de6-891f-713045c4c4e5)

Задание 2 

Тут с помощью программы crontab мы напишем простой скрипт на выполнение ежедневноего бэкапа домашней директории в директорию tmp/backup, внутри скрипта ключами указываем: a - Режим архивирования,v - Вывод подробной информации о процессе синхронизации, 
 z - Сжимать данные файла во время передачи, r- Рекурсивный режим для каталогов, и так же --delete если я всё правильно понял с помощью этой команды созадается зеркальная копия. Процесс выполения можно посмотреть в логах cat /var/log/syslog | grep CRON 

![Снимок экрана от 2024-03-11 13-30-31](https://github.com/Niko1a/lebedev/assets/110035244/2c40c3f3-22bb-4e30-a2de-55c1933d3d61)

![Снимок экрана от 2024-03-11 13-31-48](https://github.com/Niko1a/lebedev/assets/110035244/67399d5a-9fbb-444e-80b9-67db44d44564)
