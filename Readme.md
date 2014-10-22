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
##Ensure the location of the binaries is in the PATH variable
The MongoDB binaries are in the bin/ directory of the archive. To ensure that the binaries are in your PATH, you can modify your PATH.
You can add the following line to your shell's rc file (e.g.~/.bashrc):
```
export PATH=<mongodb-install-directory>/bin:$PATH
```
Replace <mongodb-install-directory> with the path to the extracted MongoDB archive.

##Run MongoDB
###Create the data directory
Before you start MongoDB for the first time, create the directory to which the mongod process will write data. By default, the mongod process uses the /data/db directory. If you create a directory other than this one, you must specify that directory in the dbpath option when starting the mongod process later in this procedure. 
Note: In local development only, try with root if it doesn't work with your username.

The following example command creates the default /data/db directory:
```
mkdir -p /data/db
```
##foo

