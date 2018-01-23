django2.0版本参考
### install database
- <a href='https://docs.djangoproject.com/en/2.0/topics/install/#database-installation'>数据库参考</a>
### uninstall old versions of django
- use pip or easy_install
- or use >>> python -c "import django; print(django.\_\_path\_\_)"
### install django
- use pip ,virtualenv
- 指定django版本或默认最新
### 验证版本
- python -c "import django; print(django.get_version())"
- python -m django --version
### use
- 新建项目 >>> django-admin startproject proname
- 验证 >>> python manage.py runserver 默认 127.0.0.1：8000
- python manage.py runserver ip:port
### app
- django-admin startapp appname
- app具体做某些事情，可以包含在多个项目里。一个项目是配置文件和app的集合，可以包含多个app。
