Project Title
# Student Management SQL Project

Short Description - 
This project demonstrates basic SQL operations such as 
creating tables, inserting data, running queries, 
updating, and deleting records in a Student Management database.

## 📂 Project Structure

```StudentManagementSQL/
├─ scripts/
│ └─ student_management.sql 
├─ screenshots/ # Output screenshots
│ ├─ create_table_Courses.png
│ ├─ insert_data_Courses.png
│ ├─ select_all_Courses.png
│ ├─ create_table_Students.png
│ ├─ insert_data_Students.png
│ ├─ select_all_students.png
│ ├─ select_join_Query.png
│ ├─ update_Query.png
│ └─ delete_Query.png
└─ README.md ```


## 🛠 Tools & Technologies
- Snowflake SQL  
- Snowflake Web UI
- GitHub to store project  
- Screenshots to show outputs  

```
1.create table courses 

create or replace table Courses(Course_ID number primary key,Course_Name Varchar());



2.insert values
insert into Courses values(001,'English'),(002,'History'),(003,'Computer');

3.select * from Courses;

4..create table students

create or replace  table Students(Student_ID number primary key,Student_Name varchar(),Student_Age number,
Course_ID number, FOREIGN KEY (Course_ID) REFERENCES Courses(Course_ID));

5.insert values

insert into students values(9501,'John',19,001),(9502,'James',20,003),(9503,'Mary',18,003),(9504,'Annie',22,002);
6.select * from Students;

7.Select Query

select  a.Student_name,a.student_Age, b.Course_Name from students a join Courses b on a.Course_ID= b.Course_ID;

8.Update Query

update students
set Student_Age=24
where Student_name='John';

select * from Students;

9.Delete Query

delete from students
where Student_name='Annie';

select * from Students; ```


✅ How to Run

1.Open /scripts/student_management.sql in Snowflake Web UI 
2.Run queries step by step.
3.Compare outputs with screenshots in /screenshots.

📌 Summary

1.Learned basic Snowflake SQL commands: CREATE, INSERT, SELECT, UPDATE, DELETE
2.Practiced creating relational tables with foreign keys
3.Documented project with screenshots and README
4.Beginner-friendly project to showcase SQL skills



