# Part Two: Mongo DB Application


mongod
mongo
show dbs
use library 
show collections
db.authors.insert({name: “John”, age: “37”})
db.authors.insert({name: “Jane”, age: “42”, books: []})
var author = db.authors.find({age:{$gte { 
db.authors.find()
db.authors.find({name: “John”},{name: 1})
db.authors.findOne({})
db.authors.find({$ne:{name: “John"}})
db.authors.update({name: “John”},{name: “James”})
db.authors.update({name: “James”}, {$set:{name: “John, age: “37"}})
db.authors.remove({name: “John})
db.authors.remove({})
db.authors.insert({name: “John”, books: []})
db.authors.update({name: “John”},{$push: {books: “Of Mice and Men”}})
db.authors.update({name: “John”},{$push: {books: {$each: [“Grapes of Wrath”, “The Pearl”,”50 Shades of Gray"]}})
db.authors.update({name: “John”},{$pull: {books: “50 Shades of Gray”}})
db.authors.update({books:{$in:[“Of Mice and Men”, “The Pearl”]},{$set: {name: “John Steinbeck”}})
