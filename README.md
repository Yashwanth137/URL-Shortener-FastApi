# URL-Shortener-FastApi
### Overview
URL-Shortener-FastApi is a high-performance, lightweight URL-shortening service built with FastAPI, one of the fastest Python web frameworks. This project enables users to convert long URLs into short, easy-to-share links and provides the functionality to track and manage these shortened URLs efficiently.

### Features
FastAPI Framework: Utilizes the high-performance capabilities of FastAPI for rapid response times and asynchronous processing.<br>
URL Shortening: Converts long URLs into concise, shareable links.<br>
Redirection: Automatically redirects users to the original URL when they visit the shortened link.<br>
Analytics: Tracks usage statistics such as the number of clicks.<br>
RESTful API: Provides a simple, RESTful API for creating and managing shortened URLs.<br>
Persistence: Uses a database to store and manage URL mappings and statistics.<br>
Scalability: Designed to scale efficiently with increasing demand.

### Getting Started
Prerequisites<br>
Python 3.8+<br>
FastAPI<br>
Uvicorn (ASGI server)<br>
SQLAlchemy (for database interaction)<br>

### Installation
1. Clone the repository:
```
git clone https://github.com/Yashwanth137/URL-Shortener-FastApi.git
cd URL-Shortener-FastApi
```
2. Create a virtual environment:
```
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```
3. Install the dependencies:
```
pip install -r requirements.txt
```
4. Run the application:
```
uvicorn main:app --reload
```

### Usage
Access the API documentation at http://127.0.0.1:8000/docs for an interactive interface to test the endpoints.  
Use the provided endpoints to create shortened URLs, retrieve original URLs, and view analytics

### Project Structure
main.py: The entry point of the application containing the FastAPI instance.  
models.py: Contains SQLAlchemy models for the database.  
schemas.py: Defines Pydantic models for request and response validation.  
crud.py: Implements the CRUD operations for URL management.  
database.py: Configures the database connection and session.  
routers/: Contains route handlers for different API endpoints.  
### Contribution
Contributions are welcome! Please submit a pull request or open an issue to discuss your ideas for improving the project.

### License
This project is licensed under the MIT License. See the LICENSE file for details.
