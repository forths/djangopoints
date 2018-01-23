### django2.0 url与应用view配置
- 在应用views.py中新建view
- 在应用目录中新建 urls.py
  
      from django.urls import path

      from . import views

      urlpatterns = [
          path('', views.index, name='index'),
      ]
- 在项目目录下的urls.py中添加
  
      from django.urls import include, path
      from django.contrib import admin

      urlpatterns = [
          path('polls/', include('polls.urls')),
          path('admin/', admin.site.urls),
      ]
  ### path参数
  - route  url匹配模式
  - view   视图处理函数
  - kwargs 
  - name   url取名
