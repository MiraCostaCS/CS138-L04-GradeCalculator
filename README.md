# Lab 04 - Grade Calculator

_Learning Objective: demonstrate understanding of boolean logic and branching structures._

For this course we are using a grading system that may be new to you. In this lab you will be creating functions to help clarify what is needed to earn your desired course grade and a way to help you check your progress.

## Part 1

Write a function called `determine_grade` that has three parameters; number of unit deliverables (UDs), number of labs, and number of engagement points (EPs). The function should return the appropriate course letter grade: A, B, C, D, or F. Look at the table in the course syllabus for cutoff values. If none of the grades is appropriate, such as when a negative value is passed to the function, then the function should return `"error"`.

For example,

`determine_grade(3,11,42)`

would return `'C'`.

`determine_grade(1,-5,10)`

would return `"error"`.

Test your function several times in the main program by using a variety of values as arguments.

## Part 2

Write a new function called `progress_check_a` that will give the user an idea of how many unit deliverables, labs, and engagement points they should have completed to be on track for an A given the number of weeks completed in the semester.

For the number of unit deliverables, use that they are due on week 5, 9, 13, and 17. So if only 4 weeks of the semester have passed then zero are expected. However, if 15 weeks have passed then 3 UDs are expected.

For the number of labs and engagement points use the ratio of weeks completed to 16 (the number of weeks you have to complete all lab and EP assignments). Multiply that ratio by the number of required labs for an A. Similarly, multiply that ratio by the number of engagement points needed for an A.

Your function should return three integers. The first for the expected number of unit deliverables, the second for the expected number of labs, and the third for the expected number of engagement points.

For example,

```
num_weeks_completed = 4
num_UD,num_lab,num_EP = progress_check_a(num_weeks_completed)
print(f"To be on track for an A, after completing {num_weeks_completed} weeks of the semester you should have {num_UD} unit deliverables completed, {num_lab} labs completed, and earned {num_EP} engagement points.")
```

Should result in the following console output:

> `To be on track for an A, after completing 4 weeks of the semester you should have 0 unit deliverables completed, 3 labs completed, and earned 11 engagement points.`

## Test and Submit

There are automated tests for this lab. You can test your code by clicking on "Check Code". When you submit, the tests will also automatically run.

## Support

If you have questions please stop by student hours, send me an email, or stop by the Learning Centers to talk to a tutor either in person or online.
