# Student-Information-System
#include <stdio.h>
#include <string.h>
#define MAX_STUDENTS 100
#define MAX_NAME_LENGTH 50
struct Student {
 int rollNumber;
 char name[MAX_NAME_LENGTH];
 int age;
float marks;
};
struct Student students[MAX_STUDENTS];
int studentCount = 0;
// Function to add a student
void addStudent() {
 if (studentCount < MAX_STUDENTS) 
 {
 printf("Enter roll number: ");
scanf("%d",&students[studentCount].rollNumber);
printf("Enter name: ");
scanf("%s",&students[studentCount].name);
printf("Enter age: ");
scanf("%d",&students[studentCount].age);
printf("Enter marks: ");
scanf("%f",&students[studentCount].marks);
 studentCount++;
 printf("Student added successfully!\n");
 }
 else
 {
 printf("Maximum student limit reached!\n");
    }
}
// Function to display all students
void displayStudents() {
if(studentCount == 0) {
printf("No students found!\n");
}
else
{
for (int i = 0; i < studentCount; i++) 
{
printf("Roll Number: %d\n", students[i].rollNumber);
 printf("Name: %s\n", students[i].name);
 printf("Age: %d\n", students[i].age);
 printf("Marks: %.2f\n", students[i].marks);
printf("------------------------\n");
        }
    }
}
// Function to search for a student by roll number
void searchStudent() {
   int rollNumber;
printf("Enter roll number to search: ");
scanf("%d", &rollNumber);
for (int i = 0; i < studentCount; i++) 
{
if (students[i].rollNumber == rollNumber) 
{
printf("Student found!\n"); printf("Roll Number: %d\n", students[i].rollNumber);
printf("Name: %s\n", students[i].name);
printf("Age: %d\n", students[i].age);
printf("Marks: %.2f\n", students[i].marks);
return;
      }
  }
printf("Student not found!\n");
}
int main() {
 int choice;
 while (1)
 {
 printf("Student Information System\n");
printf("1. Add Student\n");
printf("2. Display Students\n");
printf("3. Search Student\n");
printf("4. Exit\n");
printf("Enter your choice: "); scanf("%d", &choice);
switch (choice)
{
case 1:
addStudent();
break;
case 2:
displayStudents();
break;
case 3:
searchStudent();
break;
case 4:
printf("Exiting...\n");
return 0; default:
printf("Invalid choice! Please try again.\n");
       }
   }
   return 0;
  }
