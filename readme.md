
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

Now, run the first app to check connection:

```bash
  go run 1-\ Check\ connection\ to\ MongoDB.go

  Connected to MongoDB!
````





