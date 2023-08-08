---
layout: post
title: "Introduction to Systems Software"
subtitle: "CS 0449. Fall 2023 (Term 2241)"
---

*Systems* is a branch of computer science that focuses on the design, implementation, and analysis of complex software, hardware, and their interaction. In this course, we will explore the issues of programming a real computer system by examining the abstractions, interfaces, and design decisions that influence the way that software runs.{% marginfigure 'mf-mem' 'https://imgs.xkcd.com/comics/pointers.png' 'Pointers, [XKCD 138](https://xkcd.com/138/)'%}

## About this Page
This page will provide information regarding the things I go over in recitation. Please check back for updates regularly, especially if you miss a recitation. For other course materials including lecture slides and lab/project handouts, please see the [**course website**](https://cs0449.gitlab.io/sp2023/).

## Course Description
The purpose of this course is to provide a solid understanding of how computer systems execute programs, store information, and communicate. We will explore systems-level issues from a programmer’s view by examining the abstractions, interfaces, and design decisions that influence the way that software runs on the computer system.

The perspective we will take is one of the life cycle of a program from implementation to execution. The act of compiling and running a program, a sequence of events we often take for granted, is a complex interaction of many different components that work together to manage the computer’s resources and perform the desired task.

## Contact Information
**Shinwoo Kim**<br/>
E-mail: [`shinwookim@pitt.edu`](mailto:shiwookim@pitt.edu)<br/>
Home Page: [`https://pitt.edu/~shk148/`](https://pitt.edu/~shk148/)<br/>
Office: [Fall 2023 Office Hours](https://pitt.edu/~shk148/teaching/#OH){% sidenote "office hours" "Happy to meet by appointment. Just send me an E-mail!"%}{%sidenote "tutors" "If you think you need extra help, the CS department offers *Peer Tutoring*. Sign up for an appointment on [**Navigate**](https://pitt.guide.eab.com/)."%}

## Recitations
My recitation sections accompany professor **Luis Oliveira**'s lecture **section 1090** which meets Tuesdays and Thursdays 2:30–3:45pm in the 405 Information Science Building. We will meet **every Friday at 12:00 PM in [5502 Information Science Building](https://map.concept3d.com/?id=1315#!m/386791)** unless announced otherwise.

You may attend **only** the recitation section you are signed up for unless you have received permission from the course instructor. 


<h2 id="handouts">Schedule & Handouts</h2><label for="Additional-Resources" class="margin-toggle">

{%marginnote "extra-resources" "**Additional Resources**<br>[Recommended Books/Resources on *Computer Systems*](books.html)<br>[Recommended Books/Resources on *C Programming*](c-books.html)<br>[Pitt Course Recommendations](more-systems.html)<br><br>[*How do computers read code?* (Video)](https://www.youtube.com/watch?v=QXjU9qTsYCc)<br>[*A Talk on Slab Allocators* (Video)](https://youtu.be/UQVd9mZr-jI)<br>[*The C Programming Language: Brian Kernighan* (Video)](https://youtu.be/de2Hsvxaf8M)<br>[*The Unix Operating System* (Video)](https://youtu.be/tc4ROCJYbm0)<br>[The Development of the C Language](CHistory.html)<br><br>[*Command Line Help* (Web)](https://cheatography.com/davechild/cheat-sheets/linux-command-line/)<br>[*GDB Cheatsheet* (PDF)](https://darkdust.net/files/GDB%20Cheat%20Sheet.pdf)<br>[*Vim-Adventure: A New Way To Learn Vim* (Web)](https://vim-adventures.com/)" %}


| Week | Date       | Topic                                                     | Handouts |
| ---- | ---------- | --------------------------------------------------------- | -------- |
| 00   | January 13 | **No Recitation**                                         |          |
| 01   | January 13 | **Hello Lab**<br>Getting up to speed with the environment | -        |
{: .table .table-hover}

---

## Classroom Technologies
Throughout the semester, we will be using the following resources and technologies:

### ***Discord***
[Discord](https://discord.com/) is an instant-messaging platform (similar to Skype, Microsoft Teams, and Slack) we will be using for announcements and communication. Here, you can ask your questions, get help on assignments, or socialize with your classmates.{%sidenote "faster-help" "If you ask a question on Discord, you may well get a response from one of your classmates faster than if you were to email the teaching staff."%}

The link to join the server will be posted on the [Canvas](canvas.pitt.edu) page within the first few days of term's start. You should join promptly as the link automatically expires after fourteen days.

Note that there are some guidelines about asking for help through Discord. Please review the 
academic integrity section on the syllabus carefully.

### ***Poll Everywhere***
{%marginfigure "PEV" "https://www.nova.edu/lec/This-Week-in-the-LEC/newsletter/images/survey.png" "Example of a [Poll Everywhere](https://pollev.com/home) Question"%}[Poll Everywhere](https://pollev.com/home) is a platform that we will be using for for administering in-class practice questions. You may create an account if you wish, but this is not required. During recitation, you can log in on a computer, on your phone.

PE questions are not counted for a grade, meaning you can answer them freely without worrying about getting the question wrong.

### ***Gradescope***
[GradeScope](https://www.gradescope.com/) is a tool designed to streamline and standardize assignment grading. You should create an account and link it to your Canvas classroom.{%sidenote "canvas-gs" "You can do this by clicking on the `GradeScope` link in Canvas' sidebar" %}. This is where you will submit all the work (electronically) for this course; you will find deadlines for assignments and grade on there as well.

Often, an autograder will be provided on GradeScope which gives you access to (almost) instantaneous feedback. This means you are able to make changes to your code and improve your score if you do not do well the first (or the first few) time provided there is time left before the deadline{%sidenote "add-test" "NOTE. We reserve the right to add or modify any additional test cases *after* the deadline has passed." %}.
![GradeScope Autograder Screenshot](https://cdn.gradescope.com/assets/help_center/programming-assignment-student-autograder-results-ececd41778a14c19354e3936708610dc2d67ae7c7da1937dc43f7d4cf5472e2f.png) 

As such, you should start your projects and labs early!

<style>
  table tr td, table tr th{
    background-color: rgba(0,0,0, 0) !important;
  }
  td a {
    text-shadow: none !important;
  }
</style>

