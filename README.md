# djangotest
Django фреймворкінде студенттердің топпен жұмыс жасауын тексеру мақсатында құрылған проект. 
Проектіні өз компьютеріне клондап алғаннан кейін деректер қорымен байланысу үшін төмендегі баптауларды сізге қажетті
мәндерге өзгертесіздер:
```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'djangotest_db',
        'USER':'root',
        'PASSWORD':'123',
        'HOST':'127.0.0.1',
        'PORT':'3306'
    }
}
```
Одан кейін төмендегі коммандаларды орындап шығуларыңыз қажет:
```python
python manage.py migrate
pythona manage.py makemigrations
python manage.py migrate

python manage.py createsuperuser
```
Проектіні қосып http://localhost:8000 тексеріп көріңіздер. Сізде бос экран шығады. Категорияларды деректер қорына енгізу үшін 
http://localhost:8000/admin сілтемесі бойынша категорияға қатысты деректерді сақтаймыз. Енді басты бетті қайта ашсаңыздар 
категориялар тізімі шығуы тиіс.
