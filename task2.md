## попытайтесь запустить кластер напишите получилось или нет и почему
#### Не получилось, the service did not take the steps required by its unit configuration
#### Перезапуск сервера помог, сервис запустился.
## перенесите содержимое /var/lib/postgresql/15 в /mnt/data - mv /var/lib/postgresql/15 /mnt/vdb1
## попытайтесь запустить кластер - sudo -u postgres pg_ctlcluster 15 main start
#### Job for postgresql@16-main.service failed because the service did not take the steps required by its unit configuration.
#### See "systemctl status postgresql@16-main.service" and "journalctl -xeu postgresql@16-main.service" for details.
## задание: найти конфигурационный параметр в файлах раположенных в /etc/postgresql/14/main который надо поменять и поменяйте его
#### поменял параметр data_directory на data_directory = '/mnt/vdb1/16/main'. Сервер стартовал. Табличка селектится. 


