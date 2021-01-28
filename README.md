# NMAP SCANNER GOLANG

Pre-Requisites
Go 1.10 or higher. We aim to support the 3 latest versions of Go.
MySQL installed
Nmap command line installed.

Building and Running the project
Extract the zip folder and place it under your go src directory. 

Run the sql scripts provided for DB and tables setup in the file db.sql

You can use the code editor like VScode or below commands to build and run the project.
build:  navigate to the root directory src/myproject and run- go build
run: go run hello.go
tests : go test to run the test


Endpoints
localhost:9090/home - to enter and hostname/IP for running the scan and getting the response on UI
localhost:9090/getScanDetails - the json equivalent for the above where you can pass the data in headers. Sample curl below:-

curl --location --request GET 'localhost:9090/getScanDetails' \
--header 'Content-Type: application/json' \
--header 'hostname: google.com' \
--header 'Authorization: Basic Og==' \
--data-raw ''


Acknowledgements
Regexr.com - for testing and find a regex for input validation
Golang.org - official documentation for func detais


