![](https://i.imgur.com/iywjz8s.png)


# Collaborative Document Day 2 2023-03-21-ds-intermediate-python.

Welcome to The Workshop Collaborative Document.

This Document is synchronized as you type, so that everyone viewing this page sees the same text. This allows you to collaborate seamlessly on documents.

----------------------------------------------------------------------------

This is the Document for today: https://tinyurl.com/intermediate-python-2

Collaborative Document day 1: https://tinyurl.com/intermediate-python-1

Collaborative Document day 2: https://tinyurl.com/intermediate-python-2


## 👮Code of Conduct

Participants are expected to follow these guidelines:
* Use welcoming and inclusive language.
* Be respectful of different viewpoints and experiences.
* Gracefully accept constructive criticism.
* Focus on what is best for the community.
* Show courtesy and respect towards other community members.
 
## ⚖️ License

All content is publicly available under the Creative Commons Attribution License: [creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/).

## 🙋Getting help

To ask a question, just raise your hand.

If you need help from a helper, place a yellow post-it note on your laptop lid (so that it sticks out at the top). A helper will come to assist you as soon as possible.

## 🖥 Workshop website

https://esciencecenter-digital-skills.github.io/2023-03-21-ds-intermediate-python/

🛠 Setup

https://carpentries-incubator.github.io/python-intermediate-development/setup.html

:book: Lesson material
https://carpentries-incubator.github.io/python-intermediate-development

## 👩‍🏫👩‍💻🎓 Instructors

Sven van der Burg, Jaro Camphuijsen

## 🧑‍🙋 Helpers

Giulia Crocioni, Johan Hidding

## 🗓️ Agenda
* 09:30	Welcome, feedback yesterday, **eScience center introduction**, icebreaker
* 09:40	Recap exercise
* 09:50 A bit on Continuous Integration
* 10:00 Finish Section 2: Ensuring Correctness of Software at Scale' & continue on section 3: Software Development as a Process 
* 10:30	Break
* 10:40	section 3: Software Development as a Process
* 11:20 Real-world software designs 
* 11:30	Break
* 11:40	Section 4: Collaborative Software Development for Reuse
* 12:30	Lunch Break
* 13:30	Section 4: Collaborative Software Development for Reuse
* 14:30	Break
* 14:40	Section 5: Managing and Improving Software over its Lifetime
* 15:30	Break
* 15:40	Section 5: Managing and Improving Software over its Lifetime
* 16:15	Wrap-up
* 16:30	END

## 🏢 Location logistics
* Coffee and toilets are in the hallway, just outside of the classroom.
* If you leave the building, 
  be sure to be accompanied by someone from the escience center to let you back in through the groundfloor door
* For access to this floor you might need to ring the doorbell so someone can let you in
* In case of an emergency, you can exit our floor using the main staircase.
  Or follow green light signs at the ceiling to the emergency staircase.
* **Wifi**: Eduroam should work. Otherwise use the 'matrixbuilding' network, password should be printed out and available somewhere in the room.

## 🎓 Certificate of attendance
If you attend the full workshop you can request a certificate of attendance by emailing to training@esciencecenter.nl .

## :ice_cream: Icebreaker
Move around the room.

## 🔧 Exercises
Put your answers to exercises here. Forcing yourself to write down an answer helps you learn.

### Recap day 1
Think about what you learned yesterday
* What questions do you still have?
* Are there are any incremental improvements that can benefit your projects?
* What’s nice that we learnt but is overkill for your current work?

Write your thoughts here:

- Linting useful but probably overkill at this stage, Testing on the other hand I willing on the other hand I willing on the other hand I willing on the other hand I willing on the other hand I willing on the other hand I willing on the other hand I willing on the other hand I willing on the other hand I willing on the other hand I willing on the other hand I willing on the other hand I willing on the other hand I willing on the other hand I will
-
- Using git with command line seems overkill for an every day work that does not require collaborative work with a big team in a big project
- Will we see how to apply automatic linting? it so it automatically applies the lint style and not just spotting the improvements to manually change them
- Now I know virtual environments and what continues integration excatly are. I think I will be able to use everything more or less in depth during my project.
- One question I still have is to learn how to structure my code. CI is really interesting but looks slightly overkill for my current project, at least the matrix implementation. Linting seems instead immediately useful.
- I think continuous integration is very cool but might be an overkill for the current use I make of my research software, but I should get in the habit of writing at leas a few tests for the foundational function I use for data analysis. I think however the test parametrization and CI parts could be a bit better explained, especially the used syntax, that is rather new (for me at least). I found it a bit hard to generalize the concepts and think about their application in different contex.
- I will certainly use in the future PyCharm. It was more usefull than I expected. And try to add tests in my software (if time permits)
- At this point I don't have any questions. My projects can benefit from a lot we have learned yesterday, i.e. working with feature branches and testing, but also using a proper IDE. Testing seems nice, but implementing it everywhere seems like overkill to me, however, properly implementing it in some crucial repetitive steps will be very valuable!
- I really liked learning about linters. I will use them in my work for sure. I learned a bunch of functionality of VScode that I didn't know before and I will for sure be using. Also I enjoyed working with the automated tests and the continuous integration although that'd probably be overkill for the project I am in. I don't have questions about the material from yesterday. I am however looking forward to today and learning more about collaborative software development as I am not very experienced in it. 
- I liked the use of git, I never used different branches and commited everything to main before.  Somethign I was wondering, in readme files you often see these nice figures showing if tests are passed and what score the code gets based on the test coverage. 
- Testing would be very nice to implement for my own packages. I would still like to learn more about good software development practices like avoiding code smells etc
- Many ideas I encountered that I can use to improve my projects. CI seems to be an overkill in my case as I don't normally need to deploy or distribute my software live. 
- I find the linting very useful, I also appreciate the increased attention to comment conventions. I have no questions from yesterday but I do think that I would not yet be comfortable with writing my own .yml file since the language is new for me. I think that some of the testing might be slight overkill for my research right now but I do see the potential and opportunity to use it in the future.
- Git is really useful for making works more organized and it is easy to collaborate with other people.
- I enjoyed the linters and learning more about testing code. I would like to implement testing in my own project and think I have ideas on how to do it now. 
- How does the matrix CI work a bit more specifically? I could implement it as in the exercises however I think I would need a bit of more time to really understand the code and implement it for my purposes. I also think tha, at least for now, can be a bit overkill for my projects. I will definitely use the environment creation and the nice routine to use git tracking.
- I think linting and style conventions are a bit overkill, considering that there probably are more important things to focus on. Specifically, generating tests for all functions and methods seems like it should take priority. The Git and CI I will definitely introduce to my project. Especially better branching practices would be beneficial.
- I found going over style conventions, testing, and encountering CI to be very useful
- benefits of virtual environments were very clear. I'd like to learn more on this and how it compares to docker (pros and cons). General Guidelines for how to setting up in case of multiple projects along side each other      

- Learning how to branches from command line offers 


#### Temperature check 11:15

| Section     |Chapter name                                             | I am here ("x")    |
| ------      |--------                                                 | --------           |
| 2           |Automatically Testing Software                           |                    |
| 2           |Scaling Up Unit Testing                                  |                    |
| 2           |Continuous Integration for Automated Testing             |   x                 |
| 2           |Diagnosing Issues and Improving Robustness (optional)    |                    |
| 3           |Software Requirements                                    |  x  x  x              |x
| 3           |Software Architecture and Design                         | x xx  x   x  x   x        |
| 3           |Programming Paradigms                                    | x    x x      |
| 3           |Functional Programming (optional)                        |   x               x  |
| 3           |Object Oriented Programming (optional)                   |                    |
| 3           |Architecture Revisited: Extending Software (optional)    |                    |
| ?           |Somewhere else                                           |                    |


#### Temperature check 12:10

| Section     |Chapter name                                             | I am here ("x")    |
| ------      |--------                                                 | --------           |
| 2           |Automatically Testing Software                           |                    |
| 2           |Scaling Up Unit Testing                                  |                    |
| 2           |Continuous Integration for Automated Testing             |                    |
| 2           |Diagnosing Issues and Improving Robustness (optional)    |                    |
| 3           |Software Requirements                                    |                    |
| 3           |Software Architecture and Design                         | x x   x       x    |
| 3           |Programming Paradigms                                    |  x       x    x      |
| 3           |Functional Programming (optional)                        | xxxxx x   x  x  x   |
| 3           |Object Oriented Programming (optional)                   |  x        x          |
| 3           |Architecture Revisited: Extending Software (optional)    |                    |
| ?           |Somewhere else                                           |x                    |

### :scroll: Post-workshop survey
https://www.surveymonkey.com/r/JMS7HGX


### Recap day 2
Think about what you learned today
* What questions do you still have?
* Are there are any incremental improvements that can benefit your projects?
* What’s nice that we learnt but is overkill for your current work?
Consistency and style would definitely help current projects if others ever needed to understand my code. In future I may attempt to implement tests. I feel much more confident in my use of github now and the best practices for doing so.
- I have learnt a lot of useful things, e.g. linting and CI. I already had some knowledge of testing but learned new things today. Matrix CI is maybe a little overkill. Requirements is also something I'll need to think about how to apply to my work. 
- I have learned a lot on many subjects that could prove important in my everyday coding practice. CI appears to be a bit of an overkill for my current workflow. What would be interesting for a next (or different) course is some more information of the different package/environment management options, e.g. pros/cons, which could make choice more easy for the coding researcher.
- I liked the mindset that this course teaches, that software is inherently valuable and need to consider pcess things like lifetime . 
- I still don't really understand how to use the debugger and what this looks like in a regular workflow. I will add testing to my project, I found that to be useful. It was also nice to encounter some things I may not use daily (like CI) but are useful to understand.

- This was a nice to introduction to some topics such as linting and testing. Also many of the topics I had heard before but didn't need

- It was nice learn more on using git, and collaborating with other people. I would have liked to learn more on programming (functional vs OOB).



- I mainly learned about Git 
-In general I feel like I gained some 'professional' attitude towards a process that normally feels very amateur-ish when I do it. Some features feel a bit too intense for the scale I work at now, but I'm glad I know them and can work towards incorporating them.
-
- This is more a suggestion, but I would have appreciated a final summary/recap/cheat sheet with very brief list of things to consider when starting to work on a research software project (with pointers to the different sections in the lesson material to go in depth).

- Having a more grounded introduction to git (rather than just taking the plunge and trying it out) was very nice. The material on requirements, design and architecture were very useful.


## 🧠 Collaborative Q&A
Put your questions for central discussion here:

## 📚 Resources
Extra topics for fast learners:
- [Persistence (storing data in JSON)](https://carpentries-incubator.github.io/python-intermediate-development/persistence/index.html)
- [Databases](https://carpentries-incubator.github.io/python-intermediate-development/databases/index.html)

- [Nice reference if you mess up with git](https://ohshitgit.com/)
- [Nice article about static, class and abstract methods](https://julien.danjou.info/guide-python-static-class-abstract-methods/)
- [Stackoverflow post about how to test for console print statements](https://stackoverflow.com/questions/33767627/python-write-unittest-for-console-print)
