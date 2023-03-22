# ![](https://i.imgur.com/iywjz8s.png)


# Collaborative Document Day 1 2023-03-21-ds-intermediate-python.

Welcome to The Workshop Collaborative Document.

This Document is synchronized as you type, so that everyone viewing this page sees the same text. This allows you to collaborate seamlessly on documents.

----------------------------------------------------------------------------

This is the Document for today: https://tinyurl.com/intermediate-python-1

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

If you need help from a helper, place a yellow post-it note on your laptop lid. A helper will come to assist you as soon as possible.

## 🖥 Workshop website

https://esciencecenter-digital-skills.github.io/2023-03-21-ds-intermediate-python/

🛠 Setup

https://carpentries-incubator.github.io/python-intermediate-development/setup.html

:book: Lesson material
https://carpentries-incubator.github.io/python-intermediate-development

## 👩‍🏫👩‍💻🎓 Instructors

Sven van der Burg, Jaro Camphuijsen

## 🧑‍🙋 Helpers

Giulia Crocioni, Sander van Rijn :mask:, Dani Bodor (Tue), Johan Hidding (Wed)

## 🗓️ Agenda
* 09:30	Welcome and icebreaker
* 09:45	Setting up Environment For Collaborative Code Development
* 10:30	Break
* 10:40	Setting up Environment For Collaborative Code Development
* 11:30	Break
* 11:40	Setting up Environment For Collaborative Code Development
* 12:30	Lunch Break
* 13:30	Ensuring Correctness of Software at Scale
* 14:30	Break
* 14:40	Ensuring Correctness of Software at Scale
* 15:30	Break
* 15:40	Software Development as a Process
* 16:15	Wrap-up
* 16:30	END

## :camera_with_flash: 
Pictures might be taken. Black cords means no photo.

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
* In your team, do a round of introductions:
  - State your name
  - One sentence for where you come from, what is your background?
  - One sentence where you are currently? What do you work on?
  - One sentence what do you wish to learn in this course?
  - In one sentence share something not a lot of people know about you.
* As a team come up with a good team name. Write it down on a blue sticky.

## 🔧 Exercises
Put your answers to exercises here. Forcing yourself to write down an answer helps you learn.

### Where are you?
Add a "x" in the table to indicate in which chapter you are currently working. 

#### Temperature check 11:30
| Chapter name                                             | I am here ("x")    |
| --------                                                 | --------           |
| Setup                                                    |                    |
| Introduction to Our Software Project                     |                    |
| Virtual Environments For Software Development            |                    |
| Integrated Software Development Environments             | X   x   x x        |
| Collaborative Software Development Using Git and GitHub  |x x x x x  x x  x   |
| Python Code Style Conventions                            |  x  x x x x x      |
| Verifying Code Style Using Linters                       | x x  x    x        |
| Somewhere else                                           |  X                 |


Try to finish section 1 by 14:30. The "Verifying Code Style Using Linters" chapter is optional  for today (you can always go back to that section after the workshop). 
After the break (at 14:40) we will start with section 2. Ask us (yellow sticky note on your laptop) or your team mates for help if you think you cannot finish in time. 

#### Temperature check 14:20

| Chapter name                                             | I am here ("x")    |
| --------                                                 | --------           |
| Setup                                                    |                    |
| Introduction to Our Software Project                     |                    |
| Virtual Environments For Software Development            |                    |
| Integrated Software Development Environments             |  x                 |
| Collaborative Software Development Using Git and GitHub  |                    |
| Python Code Style Conventions                            |   x  x x   x x  x  |
| Verifying Code Style Using Linters                       |    xx xx x  x      |
| Somewhere else                                           |   x x x x  x x x   |


#### What todo now (14:30)

Save and commit all your changes and merge push into develop and main branch.

```bash
git push -u origin style-fixes
git checkout develop
git merge style-fixes
git push origin develop
git checkout main
git merge develop
git push origin main

```

#### What to do now (14:50)
Start on section 2!
https://carpentries-incubator.github.io/python-intermediate-development/20-section2-intro/index.html


#### Temperature check 16:15

| Chapter name                                             | I am here ("x")    |
| --------                                                 | --------           |
| Automatically Testing Software                           |                    |
| Scaling Up Unit Testing                                  |    x x x x  x x    |
| Continuous Integration for Automated Testing             | x x x  x x x x x x x|
| Diagnosing Issues and Improving Robustness               |   xx  xx  x       |
| Somewhere else                                           |                    |


### :right_anger_bubble: Feedback
#### What went well? (Morning)
* moving independently through the material, steps are clear 
* working in groups, going through the exercies
* everything is very clear for once, usually all the resources on these topics are very confusing. I like the fact you acknowledge there are multiple ways to do things and try to help u
* I like the topics covered in the materials and that it is very clear
* very clear material
* clarity of what to do and when to do it / also thanks for reminding us to take breaks ☕️
* Well written and thought out exercises and other material, not too many external documents and links.
* I li


#### What can be improved? (Morning)
* Unsure how quickly / slowly to move through material, but noticed that there is a time breakdown at the top of the exericises
* I had some trouble with pycharm, now I am using VScode (lost some time there tying to use pycharm)
* Nothing so far
* I missed the part where you said where to find the lesson materials so I was just waiting for a while for the othes to finish the set up and thought you would disclose that later. Maybe you can highlight it better somewhere on this document?
 


#### What went well? (Afternoon)
* liked the introduction to pycharm and testing section. looking out to tomorrow
* very clear and useful material, testing section super useful!
* The day flew by, enjoyed the material, super useful
* Clear, yet informative instructions

#### What can be improved? (Afternoon)
* I found it a bit hard to focus with a lot of discussions going on in the room, all of which are potentially interesting so you end up listening to people next to you. I'm nots, may 

* People that were moving faster than the average were told to wait for others to catch up, but there did not seem to be any real reason to...

### FYI
* The collaborative documents will be stripped from personal information and shared with everyone.
* The lesson material will be freely available after the course. In fact, it's open source and you can even commit a pull request to improve it.

## 🧠 Collaborative Q&A
Put your questions for central discussion here. After each section we will discuss this.

## 📚 Resources
https://stackoverflow.com/questions/64715502/python-virtualenvs-bin-folder-does-not-have-python

https://www.jetbrains.com/help/pycharm/using-wsl-as-a-remote-interpreter.html#configure-wsl

Carpentries lesson on version control with git: https://swcarpentry.github.io/git-novice/
Git cheat sheet: https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet

https://education.github.com/git-cheat-sheet-education.pdf



