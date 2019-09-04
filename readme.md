# Vue js
- 1- cd to liwwa_vue
- 2- install npm
- 3- change settings in .env file
- 4- run comand >> npm install
- 5- run comand >> npm run prod
- 6- make your nginx sreve files in liwwa_vue/public folder

- 7- request create page :
${your_nginx_server}/index.html?full_name=smxks#/vue/register/create


- 8- list page :
${your_nginx_server}/index.html?full_name=smxks#/vue/register/


# API server (django)

- 1- create database and set configration in liwwa/settings.py line 105
- 2- install .pyenv (you can use venv) with python 3.5
- 3- run command (you have to change paths) >>  ~/.pyenv/versions/3.5.0/bin/pip install -r ~/django/liwwa/requirements.txt
- 4- migrate to database (you have to change paths) >> ~/.pyenv/versions/3.5.0/bin/python  ~/django/liwwa/manage.py migrate
- 5- add your host to ALLOWED_HOSTS and CORS_ORIGIN_WHITELIST
- 6- in liwwa_vue/.env change  MIX_API_URL to your api server