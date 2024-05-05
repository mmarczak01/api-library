This is a book storage application based on REST API

Display a list of books:
- GET http://localhost:5000/api/v1/books/ 
Content-Type: application/json

Display a specific book:
- GET http://localhost:5000/api/v1/books/<int:book_id> 
Content-Type: application/json

Adding a new book:
- POST http://localhost:5000/api/v1/books/
Content-Type: application/json

Example: 
{
  "id": 3,  
  “title”: “Witcher”,
  “description”: “Book telling the story of the witcher”,
  “read”: false
}

Deleting books:
- DELETE http://localhost:5000/api/v1/books/<int:book_id>

Editing an existing book:
- PUT http://localhost:5000/api/v1/books/<int:book_id>

Example:
PUT http://localhost:5000/api/v1/books/2

{
    “read”: true
}