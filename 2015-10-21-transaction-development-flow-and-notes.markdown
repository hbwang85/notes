---
layout: post
title: "Transaction development flow and notes"
date: 2015-10-21 14:18:55 +0800
comments: true
categories: 
---

## Install MongoDB on OSX
1 Update Homebrew’s package database.
In a system shell, issue the following command:

brew update
2 Install MongoDB.
You can install MongoDB via brew with several different options. Use one of the following operations:

Install the MongoDB Binaries
To install the MongoDB binaries, issue the following command in a system shell:
 
brew install mongodb

Run MongoDB

1
Create the data directory.
Before you start MongoDB for the first time, create the directory to which the mongod process will write data. By default, the mongod process uses the /data/db directory. If you create a directory other than this one, you must specify that directory in the dbpath option when starting the mongod process later in this procedure.

The following example command creates the default /data/db directory:

mkdir -p /data/db
2
Set permissions for the data directory.¶
Before running mongod for the first time, ensure that the user account running mongod has read and write permissions for the directory.

3
Run MongoDB.
To run MongoDB, run the mongod process at the system prompt. If necessary, specify the path of the mongod or the data directory. See the following examples.

Run without specifying paths
If your system PATH variable includes the location of the mongod binary and if you use the default data directory (i.e., /data/db), simply enter mongod at the system prompt:

mongod

https://docs.mongodb.org/manual/tutorial/install-mongodb-on-os-x/







