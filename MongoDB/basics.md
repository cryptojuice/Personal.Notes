MongoDB Basics
==============

**SQL To MongoDB Comparison Chart**
***

| **SQL Term** | **MongoDB Term**       |
|:------------:|:----------------------:|
| database     | database               |
| table        | collection             |
| index        | index                  |
| row          | BSON document          |
| column       | BSON field             |
| join         | embedding and linking  |
| primary key  | _id field              |
| group by     | aggregation            |

***

MongoDB is made up of databases which contain collections.
A collection is made up of documents. Each document is made 
up of fields.

**Inserting**
> use learn
> db.posts.insert({author:'Nick Robinson', title:'Working with MongoDB', text:'Today we will learn how to interact with mongoDB.'})

**Selectors**
> db.posts.find({author:'Nick Robinson'})
