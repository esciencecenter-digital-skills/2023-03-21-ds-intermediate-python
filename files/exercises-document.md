# Episode 00-setting-the-scene.md 

# Episode 10-section1-intro.md 

# Episode 11-software-project.md 



## Exercise: Have a Peek at the Data
Which command(s) would you use to list the contents or a first few lines of `data/inflammation-01.csv` file?
0,0,1,3,2,3,6,4,5,7,2,4,11,11,3,8,8,16,5,13,16,5,8,8,6,9,10,10,9,3,3,5,3,5,4,5,3,3,0,1
0,1,1,2,2,5,1,7,4,2,5,5,4,6,6,4,16,11,14,16,14,14,8,17,4,14,13,7,6,3,7,7,5,6,3,4,2,2,1,1
0,1,1,1,4,1,6,4,6,3,6,5,6,4,14,13,13,9,12,19,9,10,15,10,9,10,10,7,5,6,8,6,6,4,3,5,2,1,1,1
0,0,0,1,4,5,6,3,8,7,9,10,8,6,5,12,15,5,10,5,8,13,18,17,14,9,13,4,10,11,10,8,8,6,5,5,2,0,2,0
0,0,1,0,3,2,5,4,8,2,9,3,3,10,12,9,14,11,13,8,6,18,11,9,13,11,8,5,5,2,8,5,3,5,4,1,3,1,1,0

## Exercise: MVC Application Examples From your Work
Think of some other examples from your work or life where MVC architecture may be suitable or have a discussion
with your fellow learners.

# Episode 12-virtual-environments.md 

# Episode 13-ides.md 

>~~~
>{: .output}
>
> Finally, if you look at both the contents of `venv/lib/python3.9/site-packages` and `requirements.txt` and compare that with the packages shown in PyCharm's Python Interpreter Configuration - you will see that they all
> contain equivalent information.

>~~~

# Episode 14-collaboration-using-git.md 

# Episode 15-coding-conventions.md 

> ## Solution
> Modify `inflammation-analysis.py` from PyCharm, which is helpfully marking inconsistencies with
> coding guidelines by underlying them. There are a few things to fix in `inflammation-analysis.py`, for example:
>
>  1. Line 24 in `inflammation-analysis.py` is too long and not very readable. A better style would be to use
>  multiple lines and
>  hanging indent, with the closing brace `}' aligned either with the first non-whitespace character of the last line of
>  list or the first character of the line that starts the multiline construct or simply moved to the end of the
>  previous line. All three acceptable modifications are shown below.
>
>      ~~~
>      # Using hanging indent, with the closing '}' aligned with the first non-blank character of the previous line
>      view_data = {
>          'average': models.daily_mean(inflammation_data),
>          'max': models.daily_max(inflammation_data),
>          'min': models.daily_min(inflammation_data)
>          }
>      ~~~
>      {: .language-python}
>
>      ~~~
>      # Using hanging indent with the, closing '}' aligned with the start of the multiline contruct
>      view_data = {
>          'average': models.daily_mean(inflammation_data),
>          'max': models.daily_max(inflammation_data),
>          'min': models.daily_min(inflammation_data)
>      }
>      ~~~
>      {: .language-python}
>
>      ~~~
>      # Using hanging indent where all the lines of the multiline contruct are indented except the first one
>      view_data = {
>          'average': models.daily_mean(inflammation_data),
>          'max': models.daily_max(inflammation_data),
>          'min': models.daily_min(inflammation_data)}
>      ~~~
>      {: .language-python}
>
>  2. Variable 'InFiles' in `inflammation-analysis.py` uses CapitalisedWords naming convention which is recommended for class names but not variable names. By convention, variable names should be in lowercase with optional underscores so you should rename the variable 'InFiles' to, e.g., 'infiles' or 'in_files'.
>
>  3. There is an extra blank line on line 20 in `inflammation-analysis.py`. Normally, you should not use blank
> lines in the
> middle of the code unless you want to separate logical units - in which case only one blank line is used.
> Note how PyCharm is warning us by underlying the whole line.
>
>  4. Only one blank line after the end of definition of function `main` and the rest of the code on line 30 in
> `inflammation-analysis.py` - should be two blank lines. Note how PyCharm is warning us by underlying the whole line.
>
> Finally, let's add and commit our changes to the feature branch. We will check the status of our working directory first.
>
> ~~~
> $ git status
> ~~~
> {: .language-bash}
> ~~~
> On branch style-fixes
> Changes not staged for commit:
> (use "git add <file>..." to update what will be committed)
> (use "git restore <file>..." to discard changes in working directory)
> modified:   inflammation-analysis.py
>
> no changes added to commit (use "git add" and/or "git commit -a")
> ~~~
> {: .output}
>
> Git tells us we are on branch `style-fixes` and that we have unstaged and uncommited
> changes to `inflammation-analysis.py`. Let's commit them to the local repository.
> ~~~
> $ git add inflammation-analysis.py
> $ git commit -m "Code style fixes."
> ~~~
> {: .language-bash}

## Optional Exercise: Improve Code Style of Your Other Python Projects
If you have another Python project, check to which extent it conforms to PEP8 coding style.

## Exercise: Fix the Docstrings
Look into `models.py` in PyCharm and improve docstrings for functions `daily_mean` ,`daily_min`, `daily_max`.
Commit those changes to feature branch `style-fixes`.
> Once we are happy with modifications, as usual before staging and commit our changes, we check the status of our working directory:
> ~~~
> $ git status
> ~~~
> {: .language-bash}
> ~~~
> On branch style-fixes
> Changes not staged for commit:
> (use "git add <file>..." to update what will be committed)
> (use "git restore <file>..." to discard changes in working directory)
> modified:   inflammation/models.py
>
> no changes added to commit (use "git add" and/or "git commit -a")
> ~~~
> {: .output}
>
> As expected, Git tells us we are on branch `style-fixes` and that we have unstaged and uncommited
> changes to `inflammation/models.py`. Let's commit them to the local repository.
> ~~~
> $ git add inflammation/models.py
> $ git commit -m "Docstring improvements."
> ~~~
> {: .language-bash}

# Episode 16-verifying-code-style-linters.md 

## Exercise: Further Improve Code Style of Our Project
Select and fix a few of the issues with our code that Pylint detected. Make sure you do not break the rest of the
code in the process and that the code still runs. After making any changes, run Pylint again to verify you've
resolved these issues.

## Optional Exercise: Improve Code Style of Your Other Python Projects
If you have a Python project you are working on or you worked on in the past, run it past Pylint to see what issues
with your code are detected, if any.

# Episode 20-section2-intro.md 

# Episode 21-automatically-testing-software.md 

## Exercise: Write Some Unit Tests

We already have a couple of test cases in `test/test_models.py` that test the `daily_mean()` function. Looking at `inflammation/models.py`, write at least two new test cases that test the `daily_max()` and `daily_min()` functions, adding them to `test/test_models.py`. Here are some hints:

- You could choose to format your functions very similarly to `daily_mean()`, defining test input and expected result arrays followed by the equality assertion.
- Try to choose cases that are suitably different, and remember that these functions take a 2D array and return a 1D array with each element the result of analysing each *column* of the data.

Once added, run all the tests again with `python -m pytest tests/test_models.py`, and you should also see your new tests pass.



# Episode 22-scaling-up-unit-testing.md 

## Exercise: Write Parameterised Unit Tests

Rewrite your test functions for `daily_max()` and `daily_min()` to be parameterised, adding in new test cases for each of them.



# Episode 23-continuous-integration-automated-testing.md 

# Episode 24-diagnosing-issues-improving-robustness.md 

## Exercise: Exploring Tests for Edge Cases

Think of some more suitable edge cases to test our `patient_normalise()` function and add them to the parametrised tests. After you have finished remember to commit your changes.



## Optional Exercise: Add a Precondition to Check the Correct Type and Shape of Data

Add preconditions to check that data is an `ndarray` object and that it is of the correct shape.
Add corresponding tests to check that the function raises the correct exception.
You will find the Python function [`isinstance`](https://docs.python.org/3/library/functions.html#isinstance)
useful here, as well as the Python exception [`TypeError`](https://docs.python.org/3/library/exceptions.html#TypeError).
Once you are done, commit your new files, and push the new commits to your remote repository on GitHub.



## Exercise: Fix Code Style Errors

Rename our local variable `max` to something else (e.g. call it `max_data`), then rerun your tests and
commit these latest changes and
push them to GitHub using our usual feature branch workflow. Make sure your `develop` and `main` branches are up to date.

# Episode 30-section3-intro.md 

# Episode 31-software-requirements.md 

## Exercise: New Business Requirements
Think of a new hypothetical business-level requirements for this software. This can be anything you like, but be sure to keep it at the high-level of the business itself.
> ## Solution
> One hypothetical new business requirement (BR3) could be extending our clinical trial system to
> keep track of doctors who are being involved in the project.
>
> Another hypothetical new business requirement (BR4) may be adding a new parameter to the treatment and checking if improves
> the effect of the drug being tested - e.g. taking it in conjunction with omega-3 fatty acids and/or increasing physical activity
> while taking the drug therapy.

## Exercise: New User Requirements

Break down your new business requirements from the [previous exercise](../31-software-requirements/index.html#exercise-new-business-requirements)
into a number of logical user requirements, ensuring they stay above the level and detail of implementation.
> ## Solution
> For our business requirement BR3 from the previous exercise, the new user/stakeholder requirements may be the ability to
> see all the patients a doctor is being responsible for (UR3.1), and to find out a doctor looking after any individual patient (UR3.2).
>
> For our business requirement BR4 from the previous exercise, the new user/stakeholder requirements may be the ability to
> see the effect of the drug with and without the additional parameters in all reports and graphs (UR4.1).

## Exercise: Types of Software

Think about some software you are familiar with (could be software you have written yourself or by someone else) and how the environment it is used in have affected its design or development.
Here are some examples of questions you can use to get started:

- What environment does the software run in?
- How do people interact with it?
- Why do people use it?
- What features of the software have been affected by these factors?
- If the software needed to be used in a different environment, what difficulties might there be?

Some examples of design / development choices constrained by environment might be:

- Mobile Apps
- Must have graphical interface suitable for a touch display
- Usually distributed via a controlled app store
- Users will not (usually) modify / compile the software themselves
- Should work on a range of hardware specifications with a range of Operating System (OS) versions
- But OS is unlikely to be anything other than Android or iOS
- Documentation probably in the software itself or on a Web page
- Typically written in one of the platform preferred languages (e.g. Java, Kotlin, Swift)
- Embedded Software
- May have no user interface - user interface may be physical buttons
- Usually distributed pre-installed on a physical device
- Often runs on low power device with limited memory and CPU performance - must take care to use these resources efficiently
- Exact specification of hardware is known - often not necessary to support multiple devices
- Documentation probably in a technical manual with a separate user manual
- May need to run continuously for the lifetime of the device
- Typically written in a lower-level language (e.g. C) for better control of resources


## Exercise: New Solution Requirements
Now break down your new user requirements from the
[earlier exercise](../31-software-requirements/index.html#exercise-new-user-requirements)
into a number of logical solution requirements (functional and non-functional), that address the detail required to be able to implement them in the software.
> ## Solution
> For our new hypothetical business requirement BR3, new functional solution requirements could be extending
> the clinical trial system to keep track of:
> - the names of all patients (SR3.1.1) and doctors (SR3.1.2) involved in the trial
> - the name of the doctor for a particular patient (SR3.1.3)
> - a group of patients being administered by a particular doctor (SR3.2.1).

## Optional Exercise: Requirements for Your Software Project

Think back to a piece of code or software (either small or large) you've written, or which you have experience using. First, try to formulate a few of its key business requirements, then derive these into user and then solution requirements (in a similar fashion to the ones above in *Types of Requirements*).

# Episode 32-software-design.md 

## Exercise: Implementing Requirements
Pick one of the requirements SR1.1.1 or SR1.2.1 above to implement and create an appropriate feature branch -
e.g. `add-std-dev` or `add-view` from your most up-to-date `develop` branch.

One aspect you should consider first is whether the new requirement can be implemented within the existing design. If not, how does the design need to be changed to accommodate the inclusion of this new feature? Also try to ensure that the changes you make are amenable to unit testing: is the code suitably modularised such that the aspect under test can be easily invoked with test input data and its output tested?

If you have time, feel free to implement the other requirement, or invent your own!

Also make sure you push changes to your new feature branch remotely to your software repository on GitHub.

**Note: do not add the tests for the new feature just yet - even though you would normally add the tests along
with the new code, we will do this in a later episode. Equally, do not merge your changes to the
`develop` branch just yet.**

**Note 2: we have intentionally left this exercise without a solution to give you more freedom in implementing it how you see fit. If you are struggling with adding a new view and command line parameter, you may find the standard deviation requirement easier. A later episode in this section will look at how to handle command line parameters in a scalable way.**

# Episode 33-programming-paradigms.md 

# Episode 34-functional-programming.md 

## Exercise: Pure Functions

Which of these functions are pure?
If you're not sure, explain your reasoning to someone else, do they agree?

~~~
def add_one(x):
return x + 1

def say_hello(name):
print('Hello', name)

def append_item_1(a_list, item):
a_list += [item]
return a_list

def append_item_2(a_list, item):
result = a_list + [item]
return result
~~~


## Exercise: Check Inflammation Patient Data Against A Threshold Using Map
Write a new function called `daily_above_threshold()` in our inflammation `models.py` that determines whether or not
each daily inflammation value for a given patient exceeds a given threshold.

Given a patient row number in our data, the patient dataset itself, and a given threshold, write the function to use `map()` to generate and return a list of booleans, with each value representing whether or not the daily inflammation value for that patient exceeded the given threshold.

Ordinarily we would use Numpy's own `map` feature, but for this exercise, let's try a solution without it.

## Exercise: Calculate the Sum of a Sequence of Numbers Using Reduce
Using reduce calculate the sum of a sequence of numbers. Although in practice we would use the built-in `sum()` function for this - try doing it without it.

## Exercise: Extend Inflammation Threshold Function Using Reduce
Extend the `daily_above_threshold()` function you wrote previously to return a count of the number of days a patient's inflammation is over the threshold. Use `reduce()` over the boolean array that was previously returned to generate the count, then return that value from the function.

You may choose to define a separate function to pass to `reduce()`, or use an inline lambda expression to do it (which is a bit trickier!).

Hints:
- Remember that you can define an `initialiser` value with `reduce()` to help you start the counter
- If defining a lambda expression, note that it can conditionally return different values using the syntax `<value> if <condition> else <another_value>` in the expression.

Where could this be useful? For example, you may want to define the success criteria for a trial if, say, 80% of
patients do not exhibit inflammation in any of the trial days, or some similar metrics.

## Exercise: Measuring Performance Using Decorators
One small task you might find a useful case for a decorator is measuring the time taken to execute a particular function. This is an important part of performance profiling.

Write a decorator which you can use to measure the execution time of the decorated function using the [time.process_time_ns()](https://docs.python.org/3/library/time.html#time.process_time_ns) function. There are several different timing functions each with slightly different use-cases, but we won’t worry about that here.

For the function to measure, you may wish to use this as an example:
~~~
def measure_me(n):
total = 0
for i in range(n):
total += i * i

return total
~~~

# Episode 35-object-oriented-programming.md 

## Exercise: Structuring Data

Write a function, called `attach_names`, which can be used to attach names to our patient dataset.
When used as below, it should produce the expected output.

If you're not sure where to begin, think about ways you might be able to effectively loop over two collections at once.
Also, don't worry too much about the data type of the `data` value, it can be a Python list, or a NumPy array - either is fine.

~~~ python
data = np.array([[1., 2., 3.],
[4., 5., 6.]])

output = attach_names(data, ['Alice', 'Bob'])
print(output)
~~~

~~~
[
{
'name': 'Alice',
'data': [1., 2., 3.],
},
{
'name': 'Bob',
'data': [4., 5., 6.],
},
]
~~~


## Exercise: A Basic Class

Implement a class to represent a book.
Your class should:

- Have a title
- Have an author
- When printed using `print(book)`, show text in the format "title by author"

~~~ python
book = Book('A Book', 'Me')

print(book)
~~~

~~~
A Book by Me
~~~


## Exercise: A Model Patient

Let's use what we have learnt in this episode and combine it with what we have learnt on
[software requirements](../31-software-requirements/index.html) to formulate and implement a
[few new solution requirements](../31-software-requirements/index.html#exercise-new-solution-requirements)
to extend the model layer of our clinical trial system.

Let's can start with extending the system such that there must be a `Doctor` class to hold the data representing a single doctor, which:
- must have a `name` attribute
- must have a list of patients that this doctor is responsible for.

In addition to these, try to think of an extra feature you could add to the models which would be useful for managing a dataset like this - imagine we're running a clinical trial, what else might we want to know?
Try using Test Driven Development for any features you add: write the tests first, then add the feature.
The tests have been started for you in `tests/test_patient.py`, but you will probably want to add some more.

Once you've finished the initial implementation, do you have much duplicated code?
Is there anywhere you could make better use of composition or inheritance to improve your implementation?

For any extra features you've added, explain them and how you implemented them to your neighbour.
Would they have implemented that feature in the same way?
return new_observation

# Episode 36-architecture-revisited.md 

# Episode 40-section4-intro.md 

# Episode 41-code-review.md 



## Exercise: Implement Tests for the New Feature
Look back at the [solution requirements](/31-software-requirements/index.html#solution-requirements) (SR1.1.1 or SR1.2.1) for
the feature that was implemented in your shared repository. Implement tests against the appropriate
specification in your local feature branch.

*Note: Try not to not fall into the trap of writing the tests to test the existing code/implementation - you should
write the tests to make sure the code satisfies the requirements regardless of the actual implementation. You can
treat the implementation as a [black box](https://en.wikipedia.org/wiki/Black-box_testing) - a typical approach
to software testing - as a way to make sure it is properly tested against its requirements without introducing
assumptions into the tests about its implementation.*

## Exercise: Code Review in Your Own Working Environment

At the start of this episode we briefly looked at a number of techniques for doing code review, and as an example, went on to see how we can use GitHub Pull Requests to review team member code changes. Finally, we also looked at some best practices for doing code reviews in general.

Now think about how you typically develop code, and how you might institute code review practices within your own working environment. Write down briefly for your own reference (perhaps using bullet points) some answers to the following questions:

- Which 2 or 3 key circumstances would code review be most useful for you and your colleagues?
- Referring to the first section of this episode above, which type of code review would be most useful for each circumstance (and would work best within your own working environment)?
- Taking one of these circumstances where code review would be most beneficial, how would you organise such a code review, e.g.:
- Which aspects of the codebase would be the most useful to cover?
- How often would you do them?
- How long would the activity take?
- Who would ideally be involved?
- Any particular practices you would use?

# Episode 42-software-reuse.md 

## Exercise: Preparing for Release

In a (hopefully) highly unlikely and thoroughly unrecommended scenario, your project leader has informed you of the need to release your software within the next half hour, so it can be assessed for use by another team. You'll need to consider finishing the README, choosing a licence, and fixing any remaining problems you are aware of in your codebase. Ensure you prioritise and work on the most pressing issues first!

# Episode 43-software-release.md 

## Optional Exercise: Enhancing our Package Metadata

The [Python Packaging User Guide](https://packaging.python.org/) provides documentation on [how to package a project](https://packaging.python.org/en/latest/tutorials/packaging-projects/) using a manual approach to building a `pyproject.toml` file, and using Twine to upload the distribution packages to PyPI.

Referring to the [section on metadata](https://packaging.python.org/en/latest/tutorials/packaging-projects/#configuring-metadata) in the documentation, enhance your `pyproject.toml` with some additional metadata fields to improve the information your package.

# Episode 50-section5-intro.md 

# Episode 51-managing-software.md 

## Exercise: Our First Issue!
Individually, with a critical eye, think of an aspect of the code you have developed so far that needs improvement.
It could be a bug, for example, or a documentation issue with your README, a missing LICENSE file, or an enhancement.
In GitHub, enter the details of the issue and select `Submit new issue`. Add a label to your issue, if appropriate.

Time: 5 mins
> ## Solution
> For example, "Add a licence file" could be a good first issue, with a label `documentation`.

## Exercise: Our First Mention/Reference!
Add a mention to one of your team members using the `@` notation
in a comment within an issue or a pull request in your repository - e.g. to
ask them a question or a clarification on something or to do some additional work.

Alternatively, add another issue to your repository and reference the issue you created in the previous exercise using the
`#` notation.

Time: 5 mins

## Exercise: Working With Projects
Spend a few minutes planning what you want to do with your project as a bigger chunk of work (you can continue working on the
first release of your software if you like)
and play around with your project board to manage tasks around the project:
- practice adding and removing columns,
- practice adding different types of cards (notes and from already existing open issues and/or unmerged pull requests),
- practice turing cards into issues and closing issues, etc.

Make sure to add a certain number of issues to your repository to be able to use in you project board.

Time: 10 mins

# Episode 52-assessing-software-suitability-improvement.md 

## Exercise: Decide on Your Group's Repository!

You all have your code repositories you have been working on throughout the course so far. For the upcoming exercise, groups will exchange repositories and review the code of the repository they inherit, and provide feedback.

Time: 5 mins

1. Decide as a team on one of your repositories that will represent your group. You can do this any way you wish.
2. Add the URL of the repository to the section of the shared notes labelled 'Decide on your Group's Repository',
next to your team's name.

## Exercise: Conduct Assessment on Third-Party Software

*The scenario:* It is envisaged that a piece of software developed by another team will be adopted and used for the long term in a number of future projects. You have been tasked with conducting an assessment of this software to identify any issues that need resolving prior to working with it, and will provide feedback to the developing team to fix these issues.

Time: 20 mins

1. As a team, briefly decide who will assess which aspect of the repository, e.g. its documentation, tests, codebase, etc.
2. Obtain the URL for the repository you will assess from the shared notes document, in the section labelled 'Decide on your Group's Repository' - see the last column which indicates which team's repository you are assessing.
3. Conduct the assessment and register any issues you find on the other team's software repository on GitHub.
4. Be meticulous in your assessment and register as many issues as you can!

# Episode 53-improvement-through-feedback.md 

## Exercise: Estimate!

As a team go through the issues that your partner team has registered with your software repository, and quickly estimate how long each issue will take to resolve in minutes. Do this by blind consensus first, each anonymously submitting an estimate, and then briefly discuss your rationale and decide on a final estimate. Make sure these are honest estimates, and you are able to complete them in the allotted time!

Time: 15 mins

## Exercise: Prioritise!

Put your stakeholder hats on, and as a team apply MoSCoW to the repository issues to determine how you will prioritise effort to resolve them in the allotted time. Try to stick to the 60/20/20 rule, and assign all issues you'll be working on (i.e. not `Won't Haves`) to a new milestone, e.g. "Tidy up documentation" or "version 0.1".

Time: 10 mins

## Exercise: Conduct a Mini Mini-Sprint

For the remaining time in this course, assign repository issues to team members and work on resolving them as per your MoSCoW breakdown. Once an issue has been resolved, notable progress made, or an impasse has been reached, provide concise feedback on the repository issue. Be sure to add the other team members to the chosen repository so they have access to it. You can grant `Write` access to others on a GitHub repository via the `Settings` tab for a repository, then selecting `Collaborators`, where you can invite other GitHub users to your repository with specific permissions.

Time: however long is left

# Episode 60-wrap-up.md 

## Reflection Exercise: Putting the Pieces Together
As a group, reflect on the concepts (e.g. tools, techniques and practices) covered throughout the course, how they relate to one another, how they fit together in a bigger picture or skill learning pathways and in which order you need to learn them.
> ## Solution
> One way to think about these concepts is to make a list and try to organise them along two axes - 'perceived usefulness of a concept' versus 'perceived difficulty or time needed to master a concept', as shown in the table below (for the exercise, you can make your own copy of the [template table](https://docs.google.com/document/d/1NdE6PjqxjSsf1K4ofkCoWc2GA3sY2RIsjRg8BghTXas/edit?usp=sharing) for the purpose of this exercise). You then may
> think in which order you want to learn the skills and how much effort they require - e.g. start with those that are more useful but, for the time being, hold off those that are not too useful to you and take loads of time to master. You will likely want to focus on the concepts in the top right corner of the table first, but
> investing time to master more difficult concepts may pay off in the long run by saving you time and effort
> and helping reduce technical debt.
> ![Usefulness versus time to master grid](../fig/wrapup-perceived-usefulness-time.png){: .image-with-shadow width="800px"}
>
> Another way you can organise the concepts is using a [concept map](https://en.wikipedia.org/wiki/Concept_map) (a directed graph depicting suggested relationships between concepts) or any other diagram/visual aid of your choice.
> Below are some example views of tools and techniques covered in the course using concept maps. Your views
> may differ but that is not to say that either view is right or wrong. This exercise is meant to get you to reflect on what was covered in the course and hopefully to reinforce the ideas and concepts you learned.
> ![Overview of tools and techniques covered in the course](../fig/wrapup-concept-map.png){: .image-with-shadow width="800px"}
> A different concept map tries to organise concepts/skills based on their level of difficulty (novice, intermediate and advanced, and in-between!) and tries to show which skills are prerequisite for others and in which order you should consider learning skills.
> ![Overview of topics covered in the course based on level of difficulty](../fig/wrapup-concept-map-difficulty-level.png){: .image-with-shadow width="800px"}

