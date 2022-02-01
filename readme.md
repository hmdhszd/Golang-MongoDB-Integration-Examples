## Get Program

Get a copy of the program:

```bash
  git clone https://github.com/hmdhszd/Golang-MongoDB-Integration-Examples
```

Go to the project directory:

```bash
  cd Golang-MongoDB-Integration-Examples
```

## Run MongoDB

First, run MongoDB in docker:

```bash
  docker run -itd --name mongodb -p 27017:27017 ruanbekker/mongodb
```

## Run Golang Program

Then, install packages using go get:

```bash
  go mod init Golang-MongoDB

  go get go.mongodb.org/mongo-driver/mongo
````

## 1- Check connection to MongoDB

```bash
  ▶ go run 1-\ Check\ connection\ to\ MongoDB.go

  Connected to MongoDB!
````

## 2- insert a single document to MongoDB - (InsertOne)
```bash
  ▶ go run 2-\ insert\ a\ single\ document\ to\ MongoDB\ -\ \(InsertOne\).go

  Inserted a Single Document:  ObjectID("61f93dec8749b8a1f7fce114")
````




## 3- insert more than one document to MongoDB - (InsertMany) 
```bash
  ▶ go run 3-\ insert\ more\ than\ one\ document\ to\ MongoDB\ -\ \(InsertMany\)\ .go

  Inserted multiple documents:  [ObjectID("61f93e171750a6d18be19c5e") ObjectID("61f93e171750a6d18be19c5f") ObjectID("61f93e171750a6d18be19c60")]
````




## 4- Updating Documents in MongoDB
```bash
  ▶ go run 4-\ Updating\ Documents\ in\ MongoDB.go

  Matched 1 documents and updated 1 documents.
````




## 5- Find One Document in MongoDB
```bash
  ▶ go run 5-\ Find\ One\ Document\ in\ MongoDB.go 

  Found a single document: {Name:hamid Age:31 City:Paris}
````




## 6- Find Multiple Documents in MongoDB
```bash
  ▶ go run 6-\ Find\ Multiple\ Documents\ in\ MongoDB.go 
  Found multiple documents (array of pointers): [{Name:hamid Age:31 City:Paris} {Name:hamid Age:30 City:Paris} {Name:James Age:32 City:New York} {Name:Frankie Age:31 City:Vegas} {Name:hamid Age:30 City:Paris} {Name:James Age:32 City:New York} {Name:Frankie Age:31 City:Vegas} {Name:hamid Age:30 City:Paris} {Name:James Age:32 City:New York} {Name:Frankie Age:31 City:Vegas}]
  
  hamid
  31
  Paris
````




## 7- Delete One Document in MongoDB
```bash
  ▶ go run 7-\ Delete\ One\ Document\ in\ MongoDB.go 

  Deleted 1 documents in the trainers collection
````




## 8- Delete Many Documents in MongoDB
```bash
  ▶ go run 8-\ Delete\ Many\ Documents\ in\ MongoDB.go 

  Deleted 9 documents in the trainers collection
````