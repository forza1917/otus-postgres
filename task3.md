##sudo -iu postgres pgbench -i
#### таблицы созданы, 14 версия postgresql
## до настроек tps = 587.0  
#### Необходимые настройки: 
## DB Version: 14
## OS Type: linux
## DB Type: dw
## Total Memory (RAM): 8 GB
## CPUs num: 2
## Data Storage: ssd
## max_connections = 40
## shared_buffers = 2GB
## effective_cache_size = 6GB
## maintenance_work_mem = 1GB
## checkpoint_completion_target = 0.9
## wal_buffers = 16MB
## default_statistics_target = 500
## random_page_cost = 1.1
## effective_io_concurrency = 200
## work_mem = 13107kB
## huge_pages = off
## min_wal_size = 4GB
## max_wal_size = 16GB
## после настроек tps = 227.885428
## устанавливаем pgbadger и lynx, смотрим out.html
## Добавляем ramdisk  /tmp/disk/mem/1gb/ tmpfs defaults,size=1G,x-gvfs-show  0  0
## Для ускорения отключаем автовакуум - autovacuum = off

