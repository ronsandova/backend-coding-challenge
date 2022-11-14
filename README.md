# Backend development task

The challenge requires you to create a small API which has 3 o 4 main functions, create a new program, create a new program intake, create a new student, and enrol a student into a program. For the purpose of this exercise, storing the created records in a database is not required, however experience dealing with SQL is required for this role, so you may want to consider implementing a small SQL database such [SQLite](https://www.sqlite.org/) for this challenge.

Beside the repository conventions feel free to add functionality or relationships as you see fit.

The requirements of the spec are as follows: Ability to create a new program (programs should be run within a specified time frame e.g. jan 4th - jan 11th) Ability to create a new student and ability to enrol the student into a program (students should be able to enrol in multiple programs provided there are no clashing times)

No testing is required.

If there are ways in which you think the system could be improved/enhanced, please note it down and explain the enhancement (no need to implement it).


## Technical requirement

1. Create a  docker-compose up, to spin up any db container and a workspace for development
2. Use any NodeJS framework

## Endpoints 
 
http://localhost:3000/enroll/add (POST)
```json
 {
    "student_id": "xxxx",
    "intake_course": "xxxx",
    "course": "xxxx"
}
```

http://localhost:3000/program/add (POST)
```json
{
  "name": "Mental health consent",
  "description": "Lorem Ipsum**  is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy/"
}
```

http://localhost:3000/intake/add (POST)
```json
{
  "name": "Marrickville school year 10 first semester",
  "description": "Course Intake",
  "start_date": "2020-10-22",
  "finish_date": "2021-03-29"
}
```

http://localhost:3000/student/add (POST)

```json
{
  "email": "Joseph.Galler@gmail.com",
  "first_name": "Joseph",
  "last_name": "Galler"
}
```

Please reach out if there are any questions
