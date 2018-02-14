# Linux Server Configuration
Configured a Linux server from scratch to host database-driven web application.

## The IP address and SSH port so the server can be accessed:
Internal IP: 10.142.0.2
External IP: 35.196.156.144
SSH Port: 2200

## The complete URL to the hosted web application:
URL: http://catalog.cf

## A summary of softwares installed and configuration changes made:
1. Updated and upgraded all the system softwares.
2. Changed the ssh port from 22 to 2200 using firewall settings.
3. Created a user **grader** with sudo privilege.
4. Generated SSH key-pair to authenticate user **grader** and disabled password authentication.
5. Installed apache web server using `sudo apt-get install apache2`
6. Created the app folder **catalog** in `/var/www/` and cloned github repository.
7. Created a virtual environment and installed all the dependencies from **requirements.txt** and configured the postgresql database.
8. Created a wsgi file called `catalog.wsgi` in the directory `/var/www/catalog` to initialize the app.
9. Created **catalog.conf** and configured apache virtualhost in the directory `/etc/apache2/sites-available`
10. Restarted apache service using `sudo service apache2 restart`

## A list of any third-party resources used to complete this project:
1. Google Compute Engine
2. Apache 2
3. mod_wsgi 4.5.24


