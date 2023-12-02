# Lab Report 5

> Hello, I'm a student in CSE 15L and I'm facing some trouble with my code. When I try to run my grade.sh script, it doesn't work as expected. I believe the issue might be related to the script itself, but I'm not entirely sure what's going wrong.
> Here's what I think happens: I run the script to grade a Java assignment, but it seems to fail during the compilation stage. I'm guessing there could be something wrong with the way I'm handling file paths or dependencies in the script, but I can't pinpoint the exact problem. Can someone help me figure out what's causing this issue?


![Image](grade_symptoms.png)

> Hello student, I am a TA for CSE 15L here to help you, keeping your symptom in mind, I recommend double-checking the grade.sh script for any misused file paths or directory references, as these are common sources of errors in such scripts. Here is a command that could help you figure out what the issue is: ` bash -x grade.sh [repository link] `

![Image](after_command_run.png)

> Thank you that helped a lot! I found out that there were two bugs in my grade.sh file, the fist one was that I was that I was referencing a jar file that was not in my lib and the second one was that I was trying to copy a nonexistant file to the grading-area.

> For my grade.sh script which comes from my home directory, I also need the TestListExamples.java file, and a lib directory with JUnit and Hamcrest JAR files. The script creates student-submission and grading-area directories for cloning student repositories and compiling and running tests.

