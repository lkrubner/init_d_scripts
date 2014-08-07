init_d_scripts
==============

The init_d scripts to start/stop the LaunchOpen apps as daemons

The LaunchOpen website depends on various apps on the server, including the loupi app which offers the persistence layer, and the lo_login_service that lets users signup and login. 

What would happen if Amazon suffered a service outage and our web servers restarted, or one of the developers felt the need to restart a server? We need to ensure that the loupi app and the lo_login_service app (and other apps) restart automatically when the server restarts, so we have added some init.d scripts to ensure that the start-stop-daemon restarts these apps as daemonized services. 



