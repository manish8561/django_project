# Python Project in Django

Learning basic python project with django

## Requirements

- Docker
- Python
- Anaconda

## Setup
- commands for mysql and phpmyadmin setup in docker

```bash
docker run --name some-mysql -v /media/ishanvi/data/storages/mysql:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=root -d --rm -p 0.0.0.0:3306:3306 mysql:latest
docker run --name phpmyadmin -d --link some-mysql:db -p 8080:80 --rm phpmyadmin
```
- commands to create virtal env:
```bash
conda create --name django_env --file requirements.txt
conda activate django_env
```
-command to run project:
```bash
python manage.py runserver
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## Author

[Manish Sharma](https://github.com/manish8561/)