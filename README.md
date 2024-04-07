Requiremnts
Python
Anaconda

docker run --name some-mysql -v /media/ishanvi/data/storages/mysql:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=root -d --rm -p 0.0.0.0:3306:3306 mysql:latest
docker run --name phpmyadmin -d --link some-mysql:db -p 8080:80 --rm phpmyadmin
conda activate django_env

run command
py manage.py runserver


