## Устанавливаем postgres 15, устанавливаем pg_probackup-15
## Создаем каталог бэкапов, инициализируем его.
## Backup catalog '/home/backups' successfully initialized
## Создаем роль backup, выдаем права, инициализируем pg_probackup-15
## Создаем таблицу, снимаем полный бэкап pg_probackup-15 backup --instance 'main' -b FULL --stream --temp-slot
## Снимаем инкрементальный бэкап
## Создаем второй кластер main2
## Восстанавливаем туда из бэкапа pg_probackup-15 restore --instance 'main' -i 'S20ILS' -D /var/lib/postgresql/15/main2
## Таблица доступна
