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

Download the binary files for the latest MongoDB release.
Donwload binaries from [here](https://mongodb.org/downloads).

For example, to download the latest release through the shell, issue the following:
```
curl -O http://downloads.mongodb.org/osx/mongodb-osx-x86_64-2.6.4.tgz
```
##Extract the files from the downloaded archive
From a system shell, you can use the *tar* command:
```
tar --zxvf mongodb-osx-x86_64-2.6.4.tgz
```
##Copy the extracted archive to the target directory
Copy the extracted folder to the location from which MongoDB will run.
```
mkdir -p mongodb
cp -R -n mongodb-osx-x86_64-2.6.4/ mongodb
```
##foo

