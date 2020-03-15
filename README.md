# Blog project
This blog is for trainees

# Stack
Python 3.5 (changed because we dependent on our staging server)  
Django 2.2  
Bootstrap 4.4  

# Resources  
https://githowto.com/ - tutorial for git.  
https://nvie.com/posts/a-successful-git-branching-model/ - branching model we use.  
    In Russian (https://habr.com/ru/post/106912/)  
https://docs.djangoproject.com/en/2.2/ - django documentation.  
https://getbootstrap.com/docs/4.4/getting-started/introduction/ - bootstrap documentation.  
https://www.w3schools.com/sql/default.asp - SQL tutorial.  
https://www.w3schools.com/bootstrap4/default.asp - bootstrap tutorial.  
https://www.w3schools.com/html/default.asp - HTML tutorial.  
https://www.w3schools.com/css/default.asp - CSS tutorial.  
https://www.w3schools.com/js/default.asp - JavaScript tutorial.  

# Development setup  
Go to a directory with all your projects.
```bash  
cd /path/to/directory/with/your/projcts/
```  
Clone the project. Make sure you properly set up your ssh key for using with github.com.
```bash  
git clone git@github.com:TheFutureProofTechnology/blog.git  
```  
Go to the project directory.
```bash  
cd blog  
```  
Setup a virtual environment.
```bash  
virtualenv --python=python3.5 venv  
```  
Activate the virtual environment.
```bash  
source venv/bin/activate
```  
Install all dependencies.
```bash  
pip install -r requirements.txt
```  
Copy an environment file and setup your variables.
```bash  
cp .env.example .env
```  
Run migrations.
```bash  
./manage.py migrate
```  
Create a superuser. 
```bash  
./manage.py createsuperuser
```  
Run your dev server.
```bash  
./manage.py runserver
```  
