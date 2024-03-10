- What is MongoDb?
    - MongoDb is document oriented NoSql database.

- Sql vs NoSql Database.
    - Sql:
    1. Relational Database
    2. Table Based
    3. Not Suitable for hierarchical database
    - NoSql
    1. Non Relational Database
    2. Key-value pair
    3. Good for hierchical database
- Common MongoShell Command
    - Create Database: use myDatabae
    - Show All existing Database: show dbs
    - Current Database: db + Enter
    - Delete Database: db.dropDatabase()
    - All collections: show collections
    - Create Collections: db.createCollections("name")
    - Show all data in collection: db.users.find()
    - Find  Specific User: db.users.find({name:"Roni Hossain"}) , db.users.find({age:24}).limit(2) 
    - Update: db.users.update({name:"Roni Hossain"},{$set:{age:25}})
    - Delete: db.users.deleteOne({name:"Roni Hossain"})
- BSON vs JSON
    - JSON:
    1. JavaScript Object Notation
    2. 
- Mongoose
    - Mongooose is a ODM(Object Data Modeling) by using this we can easily connect mongosb with node.js
- Connect DB with Mongoose
    - 