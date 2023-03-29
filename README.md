# mongo-minapi-project

## Add test records to MongoDB
mongosh mongodb://root:example@mongo-db:27017
use BookStore
db.createCollection('Books')
db.Books.insertMany([{ "Name": "Design Patterns", "Price": 54.93, "Category": "Computers", "Author": "Ralph Johnson" }, { "Name": "Clean Code", "Price": 43.15, "Category": "Computers","Author": "Robert C. Martin" }])
db.Books.find().pretty()
