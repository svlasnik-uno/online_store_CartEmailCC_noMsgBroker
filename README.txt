Test
This version is updated for Django 4.0.2 and Python 3.9
This application was created as a sample by Dr. George Royce for the ISQA Web Application Development Course
To use this application:
Start PyCharm and close any projects
Select 'Get From VCS' in the upper right corner of the Pycharm window
Copy-and-paste the GitHub repository containing this project's files
Answer Yes when prompted to install requirements

Edit settings.py to add your gmail account and password for Django apps
Edit settings.py to add your personal braintree account information.


Open the Terminal Window:

Make the migrations for the database model:
   python manage.py makemigrations
   python manage.py migrate

Create a superuser:
   python manage.py createsuperuser

Run the server as Admin to make new Categories and Products.
View the application and add items to the cart.

If braintree is set up, use 4111 1111 1111 1111 as the CC# and 123 as the code with any date in the future
for an expiration date.
If braintree and your gmail are setup (gmail must be set to allow non-secure apps to have access), an
e-mail should be received with the order confirmation.
If gmail is not working, try creating an app specific password for your Google Gmail account and use that
in this application instead for gmail.


If an Error occurs when installing Pillow:
Previous Projects: If you have an error installing Pillow using Python 3.x:

To use Pillow with Python 3.8.x - upgrade pip to the most recent version (20.x)
To view the current version used by your project - execute the following command in the Terminal window (virtual
environment should be activited first)
python -m pip --version

If you have a lower version of pip - execute the following command in the Terminal window (virtual
environment should be activited first)
easy_install -U pip

Then, install the requirements for the project:
pip install -r requirements.txt

Then migrate:
python manage.py migrate
Then runserver:
python manage.py runserver
