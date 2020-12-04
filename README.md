# CrashReportsAPI

RESTful API created for managing
[**crash reports data**](https://data.world/montgomery-county-of-maryland/4df4fe03-e75b-40ef-aa92-46c06ce14fd8)
in Montgomery.

## Run API localy

```
npm start
```

## Run API on Docker

```
docker build -t docker-crash-reports-api
docker run -dp 9000:3000 docker-crash-reports-api
```

## HTTP requests

| URL             | request | functionality               |
| --------------- | ------- | --------------------------- |
| /reports/       | GET     | get all reports in a list   |
| /reports/{\_id} | GET     | get specific report by id   |
| /reports/       | POST    | submit new report           |
| /reports/{\_id} | DELETE  | remove report by id         |
| /reports/{\_id} | PUT     | update data in report by id |
