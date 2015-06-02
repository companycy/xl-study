# xl-study



start:  
gtm_ctl -Z gtm start -D /usr/local/pgsql/data_gtm ; pg_ctl start -Z datanode -D /usr/local/pgsql/data_datanode1 ; pg_ctl start -Z coordinator -D /usr/local/pgsql/data_coord1


stop:  
gtm_ctl stop -m fast -Z gtm -D /usr/local/pgsql/data_gtm ;pg_ctl stop -m fast -Z datanode -D /usr/local/pgsql/data_datanode1;  pg_ctl stop -m fast -Z coordinator -D /usr/local/pgsql/data_coord1


