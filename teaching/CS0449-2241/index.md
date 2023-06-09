---
layout: post
title: "Introduction to Systems Software"
subtitle: "CS 0449. Fall 2023 (Term 2241)"
---

{% marginfigure 'mf-mem' 'https://imgs.xkcd.com/comics/pointers.png' 'Pointers, [XKCD 138](https://xkcd.com/138/)' %}

This page will provide any information for the class that I go over in recitation. Please check back for updates regularly, especially if you miss a recitation. For other course materials including lecture slides and lab/project handouts, please see the [**course website**](https://cs0449.gitlab.io/sp2023/).

## Course Description
A *Computer System* is comprised of both hardware and software working in concert to accomplish useful work. In this course, we will explore the issues of programming a real computer system by examining the abstractions, interfaces, and design decisions that influence the way that software runs. In addition, we will look at the role of the operating system in managing system resources and providing abstractions.

## Recitation Information
<p><label for="test" class="margin-toggle"></label><input type="checkbox" id="test" class="margin-toggle" checked>
<span class="marginnote" markdown="1">
**Instructor**: Shinwoo Kim<br/>
- **E-mail**: [`shinwookim@pitt.edu`](mailto:shiwookim@pitt.edu)<br/>
- **Home Page:** [`{{site.url}}{{site.baseurl}}`]({{site.url}}{{site.baseurl}}/)<br/>
- **TA Office Hours:** [Spring 2023 Office Hours]({{ "/teaching/#OH" | absolute_url}})
</span></p>

We will meet **every Friday at 12:00 PM in 5502 [Sennott Square](https://map.concept3d.com/?id=1315#!m/376171)** unless announced otherwise. 

My recitation sections accompany professor **Luis Oliveira**'s lecture **section 1090** which meets Tuesdays and Thursdays 2:30–3:45pm in the 405 Information Science Building. You may attend **only** the recitation section you are signed up for unless you have received permission from the course instructor. 

## Classroom Technologies
To aid your learning, we will use many resources and technologies throughout the semester. 

1. The [**course website**](https://cs0449.gitlab.io/sp2023/) is where you will find all the course information, and materials such as lecture slides, lab handouts, and project directions.
2. The **class discord** is where you can ask clarifying questions, get help with assignments, and socialize with your peers. The teaching team will occasionally provide extra resources that can help your understanding (and prepare you for the exams). In addition, the teaching team will make announcements (exclusively) on Discord. CHECK FREQUENTLY!
3. [**GradeScope**](https://www.gradescope.com/) is for assignment deadlines, submissions, and grading.
4. [**Canvas**](canvas.pitt.edu) is for official grades only.
5. We will use [Poll Everywhere (PEV)](https://pollev.com/home) for interaction and participation during recitation. PEV is a classroom interaction tool (much like TopHat) that helps us guage where you are with the material. It won't be graded, but will be good practice (as most of the problems on it will be from previous exams).{%sidenote "pev" "You do not need to make an account for Poll Everywhere. You do, however, need to bring a device to recitation that is capable of connecting to the internet."%}

### Textbook and Other Resources
![CS APP](http://csapp.cs.cmu.edu/3e/images/csapp3e-cover.jpg){: height="100vh" .float-start .mx-2}The official textbook for this course is Bryant & O’Hallaron's [*Computer Systems: A Programmer's Perspective (3rd Ed)*](https://csapp.cs.cmu.edu/). It's a well written book with great explanations, but we won't be using it much.{%sidenote "CSAPP" "This is a really famous book written by [folks across 5th avenue](https://www.cmu.edu/) and is the de-facto standard when it comes to *systems textbooks*. If you are interested in how computers work (how software-hardware interact), I highly recommend giving it a read."%} Feel free to *opt-out* of textbook inclusive access if you wish.

The [*CS 0449 Book*](https://people.cs.pitt.edu/~jmisurda/teaching/cs449/cs449_latest.pdf) by Dr. Jonathan Misurda is another great book. It's based on the previous iteration of this course{%sidenote "misurda" "Previous iterations of this course had a vastly different curriculum, so you may find that some things are more/less emphasized than what we discussed in lecture. Still, this book is a great resource."%}, but has great explanations and is freely available online.

![Dive Into Systems](https://diveintosystems.org/Diveintosystemscover.jpeg){: height="100vh" .float-end .mx-2}[*Dive into Systems*](https://diveintosystems.org/book/) is a newer book that is freely available. It covers many of the topics we will discuss in this course.<span class="endmark"></span>

<br/>

---


## Student Feedback
[Please send me your anonymous feedback](https://pitt.co1.qualtrics.com/jfe/form/SV_dd9suL0AkJctj2S)
{: .text-center}

## Helpful Links
- [Sign up for **Peer Tutoring** on Navigate](https://pitt.guide.eab.com/){: target="\_blank"}
- [University of Pittsburgh](https://pitt.edu){: target="\_blank"}
- [Department of Computer Science](https://cs.pitt.edu){: target="\_blank"}
 