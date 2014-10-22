#MongoDB Basics
MongoDB is a document database. This means that we store data as
documents, which are similar to JavaScript objects. These are few sample JS objects:

```
var s = {occupation: 'engineer'};
var n = {name: 'Beatrice', grade: 12, scores:[75,87,73.5]};
```
Here's how to save a document to to a scores collection in MongoDB: then confirm that's saved properly
```
db.scores.save({p1:89});
db.scores.find();
```
##Install MongoDB on OS X
MongoDB is available through the popular OS X package manager Homebrew or through the MongoDB Download site.



