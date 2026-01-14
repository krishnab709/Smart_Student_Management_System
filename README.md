# Django Student Management System 👨‍🎓

A modern Student Management System 👨‍🎓 with features like Interactive Dashboard 🤩 Attendance Management 🏫Provide Feedback ✍ Result Generation 📜 Leave Application 🍂




Checkout the live Website [here](https://student-management-system-4jym.onrender.com/)!


### Meet the Developers ✨🌟

<table>
		<tr>
			<td align="center"><br /><sub><b>Krishnatanmay Bachhaob></sub><br/><a href="https://github.com/krishnab709">👨‍💻🚴‍♂️📸</a></td>
		  
		</tr>

</table>

## Development 👨‍💻
Note : Make sure you have Python version 3.8+



Create `.env` file (refer `.env.example` file)

Generate `SECRET_KEY` from [here](https://djecrety.ir/)

Generate your `CAPTCHA_SECRET` from [here](http://www.google.com/recaptcha/admin)

Copy your `SITE KEY` after generating `CAPTCHA_SECRET` and paste it in `data-sitekey` in `student_management_app/templates/login_page.html` (replace the current key with your key)

## Database Setup

Install Postgres Latest version from [here](https://www.postgresql.org/download/)

Install pgAdmin from [here](https://www.pgadmin.org/download/)

Create a Database using pgAdmin by following the steps mentioned [here](https://www.tutorialsteacher.com/postgresql/create-database)

Update your `DATABASE_URL` in `.env` with your DB details like `USER`, `PASSWORD` and `DB_NAME`

---

If virtualenv is not installed [(What is virtualenv?)](https://www.youtube.com/watch?v=N5vscPTWKOk&t=313s):

`$ pip install virtualenv`

Create a virtual environment

`$ virtualenv venv`

Activate the environment everytime you open the project

`$ source venv/Scripts/activate`

Install requirements 🛠

`$ pip install -r requirements.txt`

`$ pre-commit install`

Run migrations for Database

`$ python manage.py migrate`

Create superuser for Admin Login 🔐

`$ python manage.py createsuperuser`

Enter your desired username, email and password. Make sure you remember them as you'll need them in future.

eg.

    Username: admin

    Email: admin@admin.com

    Password: HighlyConfidentialPassword

All Set! 🤩

Now you can run the server to see your application up & running 🚀

`$ python manage.py runserver`

To exit the environment ❎

`$ deactivate`

Every time you want to open the application in browser, make sure you run:

`$ source venv/Scripts/activate`

`$ python manage.py runserver`

---
## Docker Setup (Optional) ![](https://skillicons.dev/icons?i=docker)

If you want to use Docker to run this project, you need to do the following steps:
- Install Docker for your OS from [here](https://www.docker.com/products/docker-desktop/)
- Run `docker --version` and `docker compose --version` [In Windows, you need to run `docker-compose --version` to check the version]
- If you see both the versions, then Docker is successfully installed on your system and you can follow along
- If you don't see the version, check with your Docker installation
- Open `docker-compose.yml` file and update the value of `CAPTCHA_SECRET` with your generated key. You can generate it from [here](http://www.google.com/recaptcha/admin) 
- Run `docker compose up -d`
- Run `docker exec -it student_management_system sh -c "python manage.py createsuperuser"` to create a new superuser
- Access the app at [http://localhost:8000](http://localhost:8000)
- To stop the container, run `docker compose stop` from the project root
- To restart the container, run `docker compose start` from the project root
- To delete the container, run `docker compose down` from the project root

---

## A Glimpse of the Dashboard 😍

![Dashboard](https://i.imgur.com/vN530l3.png)

## Stargazers

[![Stargazers](https://reporoster.com/stars/Akash1362000/Django_Student_Management_System)](https://github.com/Akash1362000/Django_Student_Management_System/stargazers)

Liked our work? 🤔 Do star [this](https://github.com/Akash1362000/Django_Student_Management_System) repository ⭐ It'll motivate us more 😁

---

### License ✍

```
MIT License

Copyright (c) 2020 Akash Shrivastava

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
