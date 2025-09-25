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
│ ├─ 1_Create_table_Courses.png
│ ├─ 2_Insert_data_Courses.png
│ ├─ 3_Select_all_Courses.png
│ ├─ 4_Create_table_Students.png
│ ├─ 5_Insert_data_Students.png
│ ├─ 6_Select_all_students.png
│ ├─ 7_Select_join_Query.png
│ ├─ 8_Update_Query.png
│ └─ 9_Delete_Query.png
└─ README.md ```


## 🛠 Tools & Technologies
- Snowflake SQL  
- Snowflake Web UI
- GitHub to store project  
- Screenshots to show outputs  

```
1.create table courses 

create or replace table Courses(Course_ID number primary key,Course_Name Varchar());

![Create Courses Table](screenshots/<img width="1920" height="963" alt="1_Create _table_Courses" src="https://github.com/user-attachments/assets/bb1272e6-66f2-4e95-aec2-b1149ae80562" />
)

2.insert values
insert into Courses values(001,'English'),(002,'History'),(003,'Computer');


![Insert Values into Courses](<img width="1920" height="960" alt="2_insert_data_Courses" src="https://github.com/user-attachments/assets/4e29f4ab-6a74-4ada-8ad1-a8875f630841" />

)

3.select * from Courses;

![Select all from Courses](<img width="1920" height="958" alt="3_Select _all_Courses" src="https://github.com/user-attachments/assets/fb69218e-d699-4177-a2b0-040c2c9679c0" />

)

4..create table students

create or replace  table Students(Student_ID number primary key,Student_Name varchar(),Student_Age number,
Course_ID number, FOREIGN KEY (Course_ID) REFERENCES Courses(Course_ID));

![Create Courses Students](<img width="1920" height="927" alt="4_Create_table _Students" src="https://github.com/user-attachments/assets/08dc9275-7d91-4526-ac5d-4529ea632e78" />

)

5.insert values

insert into students values(9501,'John',19,001),(9502,'James',20,003),(9503,'Mary',18,003),(9504,'Annie',22,002);

![Insert Values into Students](<img width="1920" height="958" alt="5_insert_data_Students" src="https://github.com/user-attachments/assets/cd418e51-428e-4554-ad26-456618eeceeb" />

)

6.select * from Students;

![Select all from Students](<img width="1920" height="940" alt="6_Select_all_Students" src="https://github.com/user-attachments/assets/c63013e0-4162-43b4-a08a-00d58483f869" />


)

7.Select Join Query

select  a.Student_name,a.student_Age, b.Course_Name from students a join Courses b on a.Course_ID= b.Course_ID;

![Select and Join Query](<img width="1920" height="960" alt="7_Select_and_Join _Query" src="https://github.com/user-attachments/assets/a20b6633-6385-4865-b94e-718b0eae8cea" />


)



8.Update Query

update students
set Student_Age=24
where Student_name='John';

![Update Query](<img width="1920" height="965" alt="8_Update_query" src="https://github.com/user-attachments/assets/9fbd65f6-35c6-47f3-a030-bac4ee95bf06" />


)


select * from Students;

9.Delete Query

delete from students
where Student_name='Annie';

![Delete Query](<img width="1920" height="949" alt="9_Delete_query" src="https://github.com/user-attachments/assets/99c9fa37-485c-4edb-a7ea-60ec20173449" />




)

select * from Students; ```


✅ How to Run

1.Open MYSQL1 in Snowflake Web UI 
2.Run queries step by step.
3.Compare outputs with screenshots in /screenshots.

📌 Summary

1.Learned basic Snowflake SQL commands: CREATE, INSERT, SELECT, UPDATE, DELETE
2.Practiced creating relational tables with foreign keys
3.Documented project with screenshots and README
4.Beginner-friendly project to showcase SQL skills



