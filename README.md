#### Upgrades
- send_confirmation instead of send_email_confirmation (remove the = in the email verification link sent to the terminal)<br>
- CustomUser Model instead of Default User<br>
- Global CSRF header for HTMX<br>
- Option to use UV for Dependency Management<br>
<br><br>


#### Getting the files
Download zip file<br> 
or<br>
run git clone command in empty folder
```bash
git clone https://github.com/dehemi2001/django_realtime_chat.git . && rm -rf .git
```
<br><br>


## Setup with UV (Recommended)


##### Install UV
uv: https://docs.astral.sh/uv/ 
```
pip install uv
```

##### Install dependencies
```
uv sync
```

##### Activate Virtual Environment (Mac)
```
source .venv/bin/activate
```

##### Migrate to database
```
python manage.py migrate
python manage.py createsuperuser
```

##### Run application
```
python manage.py runserver
```
http://localhost:8000

<br><br>


## Setup with with pip

##### Create Virtual Environment on Mac
```
python3 -m venv .venv
source .venv/bin/activate
```

##### Create Virtual Environment on Windows
```
python3 -m venv .venv
.\venv\Scripts\Activate.ps1
```

##### Install dependencies
```
pip install -r requirements.txt
pip install --upgrade pip
```

##### Migrate to database
```
python manage.py migrate
python manage.py createsuperuser
```

##### Run application
```
python manage.py runserver
```
http://localhost:8000