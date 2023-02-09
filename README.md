# EECS 489: Computer Networks (W’23)

## Administrivia
 - Lectures: 1109 FXB (Recorded), MW: 9:00 AM – 10:30 AM
 - Discussion 1: F 930-1030AM 3150 DOW
 - Discussion 2: TH 430-530PM 2153 GGBL
 - Discussion 3: F 1230-130PM 1311 EECS

### Team

| Member (uniqname) | Role | Office Hours |
| :---------------- | :--- | :----------- |
| [Z. Morley Mao](https://web.eecs.umich.edu/~zmao/) (zmao) | Faculty | [Mon 10:45-11:45am](https://officehours.it.umich.edu/queue/1293) and by appt.
| Yukun (Laura) Lou (louyukun)  | GSI | [Monday 3-5:20pm, Wed 3-3:40pm](https://officehours.it.umich.edu/queue/1295) 
| Yuanli (Leo) Zhu  (leozhu) | GSI | [Tuesday 4-6pm, (starting Feb 16: Thursday 7:30-8:30pm)](https://officehours.it.umich.edu/queue/1295)

### Piazza
All communication regarding this course must be via [Piazza](https://piazza.com/class/lc7u1gvcpzr2r6). 
This includes questions, discussions, announcements, as well as private messages.

## Course Description
EECS 489 takes a top-down approach to explore how networks operate and how network applications are written. 
We study how popular distributed systems such as video streaming, content distribution networks (CDNs), and cloud computing systems work in the *application layer*.
We explore how these applications transfer data between their components and end users over the Internet using *transport layer* protocols such as TCP and UDP.
We go deeper to understand what keeps the transport layer running (hint: the *network layer* routes packets for them); specifically, we look at how packets are routed and how routers work.
Finally, we dive one more layer down to understand how the *link layer* transfer packets using Ethernet.
In addition to cutting through the layers and covering the basics, we learn about the state-of-the-art topics in networking such as datacenter networks, software-defined networking (SDN), and programmable networks. 

From a practical point of view, we learn what sockets are and how to use them. 
And we write code. 
We write code to implement various protocols, to build client-server applications, HTTP proxies, and video distribution applications, and to learn how to use programmable networks.

### Prerequisite

The enforced prerequisite for this course is EECS 281 (Data Structures and Algorithms) and EECS 370 (Introduction to Computer Organization). 
This course does not assume or require any prior knowledge of EECS 482.
Nonetheless, you must have a good working knowledge of C/C++ and Unix family of operating systems.

### Optional Textbook

- Kurose and Ross, Computer Networking: A Top-Down Approach, 7th. or Earlier Editions, Pearson, 2016. ISBN 978-0133594140.

## Tentative Schedule

| Week of  | Monday | Wednesday | Optional Readings | Assignments
|:---------|:------:|:---------:|:------------------|:----------:
| 01/02/23 | **No Class** | [Introduction and Overview] | 1.1, 1.3, 1.4 | A1 Out
| 01/09/23 | [Protocol Layering]| [HTTP and the Web] | 1.5
| 01/16/23 | **No Class** | [DNS and CDN] | 2.2, 2.4
| 01/23/23 | [Video Streaming and Cloud Systems]| [Transport Layer]|  2.6, 3.1, 3.2, 3.3, 3.4 | A1 Due<br>A2 Out
| 01/30/23 | [TCP Basics] | [Flow and Congestion Control] | 3.5, 3.6 
| 02/06/23 | [More Congestion Control]| [Network Layer and IP] | 3.7, 4.1, 4.3.1, 4.3.2, 4.3.5
| 02/13/23 |  [IP Routers] |  [*Midterm Review*] | 4.2
| 02/20/23 | **No Class** | **MIDTERM (90 Min; Online) <br> 9 AM EDT <br>** |  | A2 Due
| 02/27/23 | **No Class** | **No Class** | | A3 Out
| 03/06/23 | [Routing Fundamentals] | [Intra-AS Routing]| 5.1, 5.2, 5.3
| 03/13/23 | [IP Addressing and Inter-AS Routing]| [BGP]| 4.3.3, 5.4
| 03/20/23 | [Software-Defined Networking] | [Link Layer] | 4.4, 5.5, 6.1, 6.3 | A3 Due<br>A4 Out
| 03/27/23 | [Switched LAN] | **No Class** | 6.4
| 04/03/23 | [Wireless Networking]| [Datacenter Networking]| 6.6, 7.1, 7.2, 7.3
| 04/10/23 | [*Final Review*] | **No Class** | 
| 04/17/23 |**No Class** | | | A4 Due
| 04/21/23 | **FINAL (90 Min; Online) <br> 9 AM EDT <br>**

## Policies

### Assignments
Four assignments will be assigned during the semester; the first one will be done individually and the rest will be in groups.
<!--- Visit [this page](Assignments) for detailed policies on assignments (including late submission policies) as well as the assignments themselves. -->

### Exams
There will be two exams during the semester: a midterm exam and the final exam. 
Both exams will be **online**.
You are expected to take both exams at the scheduled times. 

If you miss an exam for reasons other than a documented medical or personal emergency, you will receive a zero for that exam. 
If you anticipate a conflict with an exam time, talk to the instructor **at least one month** before the exam date. 
Exam dates are given at the beginning of the semester so you can avoid scheduling job interviews or other commitments on those days. 
Outside commitments are not considered a valid reason for missing an exam.

### Attendance and Discussion Sections
You are expected to attend lecture regularly and to be at your discussion section weekly. 
Discussion section meetings will typically involve active participation by discussion, group exercises, or question-and-answer sessions.

### Commitment to Equal Opportunity 
As indicated in the [General Standards of Conduct for Engineering Students](https://bulletin.engin.umich.edu/rules/#generalstandardsofconductforengineeringstudents), we are committed to a policy of equal opportunity. 
We ask that all students treat each other with respect. 
Please feel free to contact us with any problems, concerns, or suggestions.

### Lecture Recordings

Course lectures may be audio/video recorded and made available to other students in this course. As part of your participation in this course, you may be recorded. If you do not wish to be recorded, please contact `eecs489-staff-w23` the first week of class to discuss alternative arrangements.

Students may not record or distribute any class activity without written permission from the instructor, except as necessary as part of approved accommodations for students with disabilities. Any approved recordings may only be used for the student’s own private use.

## Grading
Final grades will be based on the total points earned on the assignments and exams. 
Factors such as class participation may be used to adjust your final grade, especially if it falls on a borderline. 
The tentative point breakdown is:

|              | Allocation 
| -------------| ----------:
| Assignment 1 |  5%        
| Assignment 2 | 15%        
| Assignment 3 | 15%        
| Assignment 4 | 15%        
| Midterm Exam | 25%        
| Final Exam   | 25%
| **Total**    |100%
| Quiz (Bonus) |  2%  
