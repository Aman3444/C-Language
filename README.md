# C-Language
Computer Engineering , Level - 3 , Algonquin College , Ottawa , ON 


Application design, development, debugging and testing in the Unix/Linux operating system environment are addressed. Topics covered include regular expressions, memory management, I/O and file system resources (buffered and unbuffered), and safe programming 




Programming Exercise
In this assignment, we will demonstrate what we have learned with respect to
 Using structs and arrays
 Sorting
 Code reuse
Statement of the problem
We’ll be building a simulation of a student enrolment program.
To start, you will use a list of TWELVE students.
You will represent each student by their student ID that is a randomly assigned 5-digit number, and a nested
name structure that contains their first and last name. You can arbitrarily pick a bunch of unique names for
your students.
You will create THREE courses.
You will represent each course by a name (of your choosing, e.g., “Perl Programming”); a description (of your
choosing, e.g., “Learn the fundamentals of programming scripts in Perl, and be able to...” ; a course code that
will consist of the string “CS” and a random three-digit course number (e.g., “CS193”); and the maximum
number of students that can be registered, which will be randomly set, for each course, to a number
between 4-8.
Additionally, each course will maintain the list of the students currently registered for it, and a list for those
that are on the waiting list. There is no limit to the number of students who may on the waiting list for a
course.
You will then go through the list of students, TWICE, and each pass you will randomly try to register each
student in one of the three courses. This will result in the student being either registered (if there’s room) or
put on the waiting list. A student cannot be in the same course more than once.
You will then print out the courses’ information, including registration and waiting lists. List of courses will be
sorted by the courses’ codes. You will show the number of students on each list and the capacity. Lists of
students will be sorted by the students’ ID’s.
All students will always be identified by their 5-digit student ID following by their name in the “last name, first
name” format (e.g., “78232 - Trump, Donald”)
All courses will always be identified by the course code followed by the course name, (e.g., “CS123 - Perl
Programming”).
In the descriptions above, “random” or “randomly” means that the values will be different with each
execution of the program.
You will not ever have more than one copy of a student record or course record in memory. I.e., all lists will
contain pointers to the source structures.
Optional bonus marks: Finally, you will prompt for a student ID, and print out what courses that student is
registered for, or on the waiting list for, where each course is specified by its course code and name. Entering
a zero for a student ID will exit the program.
Follow the formatting in the example below, EXACTLY. Pay attention to the nuances. Here is a sample
execution (example shows optional bonus querying).
The Output of this Assignment 


$ ./lab4.exe
CS123 – Perl Programming
Learn the fundamentals of programming scripts and be able to install Perl modules.
Registered Students (5/5):
* 00449 - Putin, Vladimir
* 11111 - Merkel, Angela
* 78232 - Donald, Trump
* 82264 - Kim, Jong-un
* 99111 - Zuma, Jacob
Waiting List (2):
* 05532 - Trudeau, Justin
* 60003 - May, Theresa
(other courses not shown for brevity)
Enter a student ID: 78232
Trump, Donald is registered for:
* CS123 – Perl Programming
* CS155 – Python for Beginners
On waiting list for:
* None
Enter a student ID: 1111
No student found with ID 1111
Enter a student ID: 11111
Merkel, Angela is registered for:
* CS123 – Perl Programming
On waiting list for:
* CS155 – Python for Beginners
Enter a student ID: 60003
May, Theresa is registered for:
* None
On waiting list for:
* CS123 – Perl Programming
* CS155 – Python for Beginners
