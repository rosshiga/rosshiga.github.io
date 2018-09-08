---
layout: essay
type: essay
title: You're Smart, What About Your Writing?
# All dates must be YYYY-MM-DD format!
date: 2018-09-06
labels:
  - S.M.A.R.T.
  - StackExchange
  - Getting help
---

Have you ever heard of [SMART goals](https://en.wikipedia.org/wiki/SMART_criteria)? SMART is a way to create goals and tasks that allow for work distribution and measured success in teams of people.

![SMART Goals via Wikipedia](../images/smart.jpg)

The reason I ask is because while I have no doubt you are smart, your goals may not be. The some of the same principles used for SMART goals can affect if people will help you and respond to questions you ask.

Specific issue questions with specific information about your environment are much more likely to get a response on public forums or mailing list. Asking questions that are targeted to a particular outcome will help you achieve that outcome. Broad questions and providing personal interjection for context information can leave readers either puzzled to the real issue or lead them down the wrong path due to bad information.

For example let’s deconstruct [this Stack Overflow question](https://stackoverflow.com/questions/3602450/where-are-my-postgres-conf-files) about postgresql, a database software. 

Kopezaur writes:
<blockquote>
I have recently reinstalled postgresql 8.3 on my Ubuntu 8.04 after update. Used EnterpriseDB package. I can connect to the database locally, I see system DB postgres but I can't configure it because I can't find config files. Searched through entire hard drive and found only samples like pg_hba.conf.sample
<br/>Where are the postgres *.conf files?
</blockquote>

You might not even have heard of postgresql before but you can quickly grasp what this question is asking for. Kopezaur is looking for the config files on Ubuntu 8.04. The context information here is great, he provides a chronologically ordered timeline of the events that lead to the posting. They also mention all the version numbers of software and what is and isn’t working along with what has been tried.

Now all of the answer are structured differently or provide different methods to access the files, but because the question is clearly written all of the responses answer the original question “Where are the postgres *.conf files?”. The most popular suggestion is to ask postgresql with a “SHOW config_file;” command because its is running. Steven Schlansker provides a different way that only works for Debian/Ubuntu, but he could answer because Kopezaur mentioned he is using Ubuntu.

Let’s be realistic here and understand that nobody is going to teach you programming without you putting in some work. Pandering to people by being self-demeaning can steer help in the other direction.  [This post](https://stackoverflow.com/questions/26291215/duplicate-error-noob-programmer) from Tiny shows that calling yourself new and inexperienced does not garner much help.

Tiny in part wrote:
<blockquote>
Here's my code, I have no idea what is wrong with it I am completely new at this and I would appreciate it a lot if I can receive some feedback thanks:)When I try to launch my app in the emulator it tells me I can't because of theses errors:
<br/>

Error:Error: Duplicate resources: C:\Users\Kam\AndroidStudioProjects\SchoolAid5\app\src\main\res\layout-ldltr-v14\activity_my.xml:layout-ldltr-v17/activity_my, C:\Users\Kam\AndroidStudioProjects\SchoolAid5\app\src\main\res\layout-ldltr\activity_my.xml:layout-ldltr-v17/activity_my
</blockquote>

First Tiny has no idea what is wrong with the program, making it sound like they haven’t done any research into the issue at all. Second, without a Git or more in-depth code samples it is near impossible to find where a duplicate resource for Android layouts might be.

This post got one response by Cory Roy that reads in part, “Looks like you may have duplicate activity_my.xml files”. Cory read the error message and basically read it back out to Tiny. The question sets the tone for the type of answers you will get.


Further reading: [How to Ask Question the Smart Way](http://www.catb.org/esr/faqs/smart-questions.html)
