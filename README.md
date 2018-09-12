# PSwitch

PSwitch is a switching application using ISO8583 Message, which has function like biller, where a client connect and pay some billing here.


## Built With

* [go](https://golang.org/doc/) - Core Framework
* [go-sql-driver](https://github.com/go-sql-driver/mysql) - Database MySQL Driver
* [jasonlvhit-gocron](https://github.com/jasonlvhit/gocron) - Scheduler
* [natefinch-lumberjack](https://github.com/natefinch/lumberjack) - Logger


### Installing

Make sure you already install go and your **$GOPATH** is right.

```
go env
```

Get and install MySQL Driver
```
go get github.com/go-sql-driver/mysql
cd $GOPATH/src/github.com/go-sql-driver/mysql
go install
```

Get and install Scheduler
```
go get github.com/jasonlvhit/gocron
cd $GOPATH/src/github.com/jasonlvhit/gocron
go install
```

Get and install Logger
```
go get github.com/natefinch/lumberjack
cd $GOPATH/src/github.com/natefinch/lumberjack
go install
```

### Build
```
cd $GOPATH/src/github.com/ivanj4u/pswitch
go install
go build
```
### Configuration
File configuration
```
cd $GOPATH/build/cfg
``` 
Here some example of configuration
```
## Application PORT
app.port=8080
app.user=aplikasi
app.pass=aplikasi123
## Database
db.url=127.0.0.1
db.port=3306
db.driver=mysql
db.dbname=api
db.user=api
db.pass=api123
``` 

### Running

Go to folder build
```
cd $GOPATH/build
``` 
Windows
```
app.exe
``` 
Linux
```
sh app
``` 

## Authors

* **Ivan Aribanilia** - *Developer* - [Githubs](https://github.com/ivanj4u)

## License

Copyright 2018 [Ivan Aribanilia](mailto:angko.j4u@gmail.com).
Please tell me if you interested with this project
