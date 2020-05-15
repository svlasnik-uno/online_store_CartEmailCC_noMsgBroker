This application was created as a sample by Dr. George Royce for the ISQA Web Application Development Course
To use this application:
Create a new Pycharm Django Project using this folder for the source.
Answer 'Yes' when prompted to use the files from this folder for the new project.
Settings: Set up the project interpreter to reference your Python 3.7 installation.
Settings: Add a new Virtual Environment

Edit settings.py to add your gmail account and password for Django apps
Edit settings.py to add your personal braintree account information.


Open the Terminal Window:

Install the required packages:
   pip install -r requirements.txt

Make the migrations for the database model:
   python manage.py migrate

Create a superuser:
   python manage.py createsuperuser

Run the server as Admin to make new Categories and Products.
View the application and add items to the cart.
If braintree is set up, use 4111 1111 1111 1111 as the CC# and 123 as the code with any date in the future 
for an expiration date.
If braintree and your gmail are setup (gmail must be set to allow non-secure apps to have access), an
e-mail should be received with the order confirmation.