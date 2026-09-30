# Student Management System Using MongoDB

A simple **Student Management System** built using **MongoDB** to demonstrate the fundamentals of NoSQL databases and MongoDB query operations.

## 📌 Project Description

This project implements a Student Management System using MongoDB. It stores student information such as **roll number, name, age, marks, and city** in a MongoDB collection.

The project demonstrates various database operations including **inserting, retrieving, updating, deleting, sorting, filtering, searching, and counting student records**. It also demonstrates MongoDB comparison and logical operators such as `$eq`, `$gt`, `$lt`, `$gte`, `$lte`, `$and`, and `$or`.

## 🚀 Features

* Create a MongoDB database
* Create a `students` collection
* Insert 50 student records
* Display all student records
* Search students by city
* Update student information
* Delete one or multiple records
* Sort students by marks
* Limit the number of displayed records
* Count documents in the collection
* Filter records using comparison operators
* Query records using `$and` and `$or`

## 🛠️ Technologies Used

* **MongoDB**
* **MongoDB Shell / mongosh**
* **NoSQL Database**

## 📂 Student Data

Each student document contains:
{
  roll: 1,
  name: "Ananya",
  age: 18,
  marks: 86,
  city: "Lucknow"
}
The project contains information for **50 students**.

## 🔍 MongoDB Operations Demonstrated

### CRUD Operations

* **Create** – Database, collection, and student records
* **Read** – Retrieve student records
* **Update** – Modify student marks/details
* **Delete** – Remove one or multiple student records

### Comparison Operators

| Operator | Purpose                  |
| -------- | ------------------------ |
| `$eq`    | Equal to                 |
| `$gt`    | Greater than             |
| `$lt`    | Less than                |
| `$gte`   | Greater than or equal to |
| `$lte`   | Less than or equal to    |

### Logical Operators

* `$and` – Matches documents where all specified conditions are true.
* `$or` – Matches documents where at least one condition is true.

## 💻 Example Queries

Find students with marks greater than 85:

db.students.find({marks: {$gt: 85}})

Find students from Lucknow:


db.students.find({city: "Lucknow"})

Find students with marks above 80 and age 19:

db.students.find({
  $and: [
    {marks: {$gt: 80}},
    {age: 19}
  ]
})

Sort students by marks in descending order:

db.students.find().sort({marks: -1})

Limit the result to 5 students:

db.students.find().limit(5)

## 🎯 Learning Objectives

The main objectives of this project are to:

* Understand NoSQL database concepts
* Learn the basic features of MongoDB
* Create databases and collections
* Perform CRUD operations
* Use MongoDB comparison operators
* Perform filtering and sorting
* Understand `$and` and `$or` operations

## 📖 Conclusion

This project provides practical experience with MongoDB and NoSQL database management. It demonstrates how MongoDB can be used to store, retrieve, modify, delete, sort, and query student records using different MongoDB operations and operators.
