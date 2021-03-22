# Wizeline QA Certification
## Assignment 2: Backend - Postman + Newman

To run the tests execute:
``` bash
newman run ./collection/Tasks.postman_collection.json -e ./env/QA_Task.postman_environment.json -r htmlextra --reporter-htmlextra-export reports/report.html
```

The report gets save inside the __reports/report.hmtl__ file.

### Bonus:
1. I would run the command as follows
``` bash
TOKEN=12345 newman run ./collection/Tasks.postman_collection.json -e ./env/QA_Task.postman_environment.json -r htmlextra --reporter-htmlextra-export reports/report.html
```
That way, I could remove the token value from any file as it will be set as an environemt variable on the process itself.