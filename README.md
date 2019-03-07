# Developer's Insight [![Build Status](https://travis-ci.com/kiamasimon/DevelopersInsight.svg?branch=master)](https://travis-ci.com/kiamasimon/DevelopersInsight)

## Advanced Django Blog Sample 
This is a beginer level project, illustrating ther basic of creating a blog and the various parts that it should include

### Getting Started
This project was implemented in the windows platform
For this project to function as intended, you must having the following installed on your machine;

    1) python 3.6
      Get it from here::https://www.python.org/downloads/
    2) Django 
      Instructions from::https://docs.djangoproject.com/en/2.1/howto/windows/
    
#### Prequisites
  1) Python has to be accessible globally 
  2) You must have created a virtual environment where the test server is to be run from.
  
#### Installing
1) Use git to clone the project to your local computer::https://github.com/rickrickysimpsoms/DjangoBlog.git.
2) Download it directly from the reopsitory.
3) Start your virtual environment.
4) Navigate to project folder where manage.py is located.
5) Run the command python manage.py runserver to start the test server and navigate to::http://localhost:8000/
    on your browser of choice.
##### Demo
   You can view the demo application from the link below:
        http://kiamasimon.pythonanywhere.com/

##### Main Urls::
    path('admin/', admin.site.urls),
    path('accounts/login/', views.LoginView.as_view(), name='login'),
    path('accounts/logout/', views.LogoutView.as_view(next_page='/'), name='logout'),
    path('', include('blog.urls')),
 ##### End Points
    path('', views.post_list, name='post_list'),
    path('post/<int:pk>/', views.post_detail, name='post_detail'),
    path('post/new/', views.post_new, name='post_new'),
    path('post/<int:pk>/edit/', views.post_edit, name='post_edit'),
    path('drafts/', views.post_draft_list, name='post_draft_list'),
    path('post/<pk>/publish/', views.post_publish, name='post_publish'),
    path('post/<pk>/remove/', views.post_remove, name='post_remove'),
    path('post/<int:pk>/comment/', views.add_comment_to_post, name='add_comment_to_post'),
    path('comment/<int:pk>/approve/', views.comment_approve, name='comment_approve'),
    path('comment/<int:pk>/remove/', views.comment_remove, name='comment_remove'),
    
#### Authors
Simon Kiama Irungu

###### Login Screen
![login screen](https://github.com/rickrickysimpsoms/DevelopersInsight/blob/master/static/images/%7B4301024D-68C5-4D57-9AD3-C04394625DEC%7D.png.jpg)

###### Landing page
![landing page](https://github.com/rickrickysimpsoms/DevelopersInsight/blob/master/static/images/%7BE8EA5359-551E-4EF2-87B9-B41C4BAF394D%7D.png.jpg)

###### Post Details page
![post details](https://github.com/rickrickysimpsoms/DevelopersInsight/blob/master/static/images/%7B6981C9CF-0957-47A0-8EE6-D2505C2040E8%7D.png.jpg)

###### Unpublished Posts page
![unpublished posts](https://github.com/rickrickysimpsoms/DevelopersInsight/blob/master/static/images/%7B7DFF65DB-FFF7-4358-9F7C-71B9A5C14B3B%7D.png.jpg)

###### Add/Edit Post page
![add/edit post](https://github.com/rickrickysimpsoms/DevelopersInsight/blob/master/static/images/%7BB8439F92-0D06-4D72-85A0-E2044FD976D8%7D.png.jpg)
