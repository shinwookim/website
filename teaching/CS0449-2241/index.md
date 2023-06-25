---
layout: post
title: "Introduction to Systems Software"
subtitle: "CS 0449. Fall 2023 (Term 2241)"
---

[Sign up for **Peer Tutoring** on Navigate](https://pitt.guide.eab.com/){: target="\_blank"}{: .text-center}

<p><label for="instr" class="margin-toggle"></label><input type="checkbox" id="instr" class="margin-toggle" checked>
<span class="marginnote" markdown="1">

**Contact Information**<br />
**Instructor**: Shinwoo Kim<br/>
**E-mail**: [`shinwookim@pitt.edu`](mailto:shiwookim@pitt.edu)<br/>
**Home Page:** [`{{site.url}}{{site.baseurl}}`]({{site.url}}{{site.baseurl}}/)<br/>
**TA Office Hours:** [Spring 2023 Office Hours]({{ "/teaching/#OH" | absolute_url}})
</span></p>

This page will provide information regarding the things I go over in recitation. Please check back for updates regularly, especially if you miss a recitation. For other course materials including lecture slides and lab/project handouts, please see the [**course website**](https://cs0449.gitlab.io/sp2023/).

## Course Description
A *Computer System* is comprised of both hardware and software working in concert to accomplish useful work. In this course, we will explore the issues of programming a real computer system by examining the abstractions, interfaces, and design decisions that influence the way that software runs. In addition, we will look at the role of the operating system in managing system resources and providing abstractions.{% marginfigure 'mf-mem' 'https://imgs.xkcd.com/comics/pointers.png' 'Pointers, [XKCD 138](https://xkcd.com/138/)' %}

## Recitation Information


We will meet **every Friday at 12:00 PM in [5502 Information Science Building](https://map.concept3d.com/?id=1315#!m/386791)** unless announced otherwise. 

My recitation sections accompany professor **Luis Oliveira**'s lecture **section 1090** which meets Tuesdays and Thursdays 2:30–3:45pm in the 405 Information Science Building. You may attend **only** the recitation section you are signed up for unless you have received permission from the course instructor. 

## Classroom Technologies
To aid your learning, we will use many resources and technologies throughout the semester. 

1. The [**course website**](https://cs0449.gitlab.io/sp2023/) is where you will find all the course information and materials such as: lecture slides, lab handouts, and project directions.
2. [**Discord**](https://discord.com/) is where you can ask clarifying questions and get help with assignments. It will also be used to provide extra resources and to make announcements.
3. [**GradeScope**](https://www.gradescope.com/) is for assignment deadlines, submissions, and grading.
4. [**Canvas**](canvas.pitt.edu) is for official grades only.
5. [**Poll Everywhere**](https://pollev.com/home) will be used for recitation participation.

### Textbook(s)

<div class="mx-auto text-center px-3" markdown="1">
[![CS APP Cover](http://csapp.cs.cmu.edu/3e/images/csapp3e-cover.jpg){: .book}](http://csapp.cs.cmu.edu/3e/home.html)
[![Misurda CS 449 Cover](misurda-cover.png){: .book}](https://people.cs.pitt.edu/~jmisurda/teaching/cs449/cs449_lainstr.pdf)
[![Dive Into Systems Cover](https://diveintosystems.org/Diveintosystemscover.jpeg){: .book}](https://diveintosystems.org/book/)
</div>


**CS:APP.** The official textbook for this course is Bryant & O’Hallaron's [*Computer Systems: A Programmer's Perspective (3rd Ed)*](http://csapp.cs.cmu.edu/3e/home.html). {%sidenote "CSAPP" "CS:APP is authored by the [people across fifth avenue](https://www.cs.cmu.edu/) and is very well-written. It provides great explanation and is the de-facto textbook when it comes to learning about computer systems. However, for this course, we will not be using it much (other than as additional reference) and you may [*opt-out*](https://solve.redshelf.com/hc/en-us/articles/360013142634-How-to-Opt-Out) of inclusive access if you wish to get a small refund."%}

**Misurda.** The [*CS 0449 Book*](https://people.cs.pitt.edu/~jmisurda/teaching/cs449/cs449_latest.pdf) by Dr. Jonathan Misurda is another great resource which is freely available online.  {%sidenote "misurda-book" "It's based on a previous iteration of this course (which had a slightly different curriculum). You may find that some things are more/less emphasized than what we discussed in lecture. Still, this book is a great resource."%}

**DIS.** [*Dive into Systems*](https://diveintosystems.org/book/) is a newer book that is also freely available. It covers many of the topics we will discuss in this course and may serve as a good resource if you want things explained in a different way.<span class="endmark"></span>

<br/>

<h2 id="handouts">Schedule <em>&</em> Handout</h2>
<style>
  table tr td, table tr th{
    background-color: rgba(0,0,0, 0) !important;
  }
  td a {
    text-shadow: none !important;
  }
</style>
<div class="table-responsive">
<table class="table table-hover bg-none">
  <thead>
<tr>
<th class="text-center">Week</th>
<th class="text-center">Date</th>
<th>Topic</th>
<th class="text-center">Handout</th>
</tr>
</thead>
<tbody>
<tr>
<td class="text-center">00</td>
<td class="text-center">January 13</td>
<td>**No Recitation**</td>
<td class="text-center">n/a</td>
</tr>

  </tbody>
</table>
</div>

### *Additional Handouts*
- [*I want to learn more about systems*...](more-systems.html)

<style>
.book{
    width: auto !important;
    height: 150px;
}
</style>