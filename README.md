# Document Manager - SoumyaRao

# Overview
This project is a simple Document Management System (DMS) built using Django and Django Rest Framework. It allows users to create, retrieve, update, and delete documents, as well as view document versions and perform certain actions like reverting to the previous version or deleting a document.

# Project Structure
- documents: Django app for handling document-related functionalities.
models.py: Defines the Document model.
serializers.py: Serializers for Document model.
views.py: API views for document-related actions.
urls.py: URL patterns for document-related endpoints.
tests.py: Testing Document Related apis


- users: Django app for user-related functionalities.
models.py: Defines the CustomUser model with password hashing methods.
serializers.py: Serializer for CustomUser model.
views.py: API views for user registration and login.
urls.py: URL patterns for user-related endpoints.
tests.py: Testing User Related apis

# Setup:
1. Clone the repository: 
git clone https://github.com/soumyaarao/PhonePe-DocumentManager-SoumyaRao
cd DocuManager

2. Install dependencies:
pip3 install -r requirements.txt

3. Apply migrations:
python3 manage.py makemigrations
python3 manage.py migrate

4. Run the development server:
python3 manage.py runserver

The server will be up and running

# API Endpoints

Document Management:
- List Documents: GET /documents/
- Create Document: POST /documents/
- List Document Versions: GET /documents/<title>/versions/
- Switch Document Version: GET /documents/<title>/versions/<version>/
- Delete Document: POST /documents/delete/
- Revert to Previous Version: POST /documents/revertlatest/

User Management:

- Register User: POST /users/register/
- User Login: POST /users/login/

# Usage
- Register a user using the POST /users/register/ endpoint.
- Log in using the POST /users/login/ endpoint.
- Use the provided endpoints for document management.

# Run the tests in the test file and enjoy!






 
