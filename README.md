# brainverse-centinum-full
Brainverse Centinum Project

Running the project locally

git clone https://github.com/briannyagol/brainverse-centinum-full.git

install virtualenv: pip install virtualenv

create a virtual environment: virtualenv project-env


on linux activate the virtualenv as shown:
source project-env/bin/activate

on windows activate the virtualenv as shown:
project-env\Scripts\activate

navigate to the project folder where the requirements.txt file exists then install all requirements:
pip install -r requirements.txt

make the initial migrations:
python manage.py makemigrations

sync the migrations with the database:
python manage.py migrate

createsuperuser:
python manage.py createsuperuser

run the server:
python manage.py runserver

Stripe and Paypal configurations:
obtain the sandbox paypal and stripe keys and update the env file

for stripe subscriptions:

add plan categories as below:
Free,
Startup,
Pro,
Enterprise

for the lists of plans add them at the stripe backend and update their IDs to the admin side




