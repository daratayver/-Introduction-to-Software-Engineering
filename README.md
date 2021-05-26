Запускать 2 процесса - джанго проект и celery.\
БД - postgres

### Системные библиотеки

sudo apt-get install mediainfo

redis

### Python либы

requirements.txt


###Добавить переменные в окружение:

###### название web-сайта
SITE_NAME=http://localhost:2000

###### случайный набор символов
SECRET_KEY=sk

###### True или False (для прода) 
DEBUG=True

###### доступ к БД
DB_NAME=evraz\
DB_USER=admin\
DB_PASSWORD=1\
DB_HOST=localhost

###### путь от корня к папке, где будут храниться видео
PATH_ROOT=/home/user/evraz/FILES

###### redis
REDIS_URL='127.0.0.1'\
REDIS_PORT=6379

###Доступ в админку:
login: superuser\
psw: 12345


пример запуска celery:\
celery -A evraz worker -B -l INFO