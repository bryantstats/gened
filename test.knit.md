---
title: "Math 201 - Final Project"
format: 
  html:
    toc: true
editor: visual
---


## Quarto

Quarto enables you to weave together content and executable code into a finished document. To learn more about Quarto see <https://quarto.org>.

## Running Code

When you click the **Render** button a document will be generated that includes both content and the output of embedded code. You can embed code like this:


::: {.cell}

```{.r .cell-code}
1 + 1
```

::: {.cell-output .cell-output-stdout}
```
[1] 2
```
:::
:::


You can add options to executable code like this


::: {.cell}
::: {.cell-output .cell-output-stdout}
```
[1] 4
```
:::
:::


The `echo: false` option disables the printing of code (only output is displayed).


## Type 1: Linear Model Projects



-------

## Type 2: Hypothesis Testing Projects
 
7. Refer to the data description in the file `HDD2015-18cy6-20-19.docx`, which variable recording the month of admission?, which variable recording the month of discharge?

8. Which month admitted the most number of patients? Which month admitted the most number of male patients?

9. Which month has the most number of teenage female patients?

10. Which provider has the most number of female patients in October? 

11. Is female patients older than male patients, on average? 

12. Calculate the average age of patients by months. Which month has the oldest patients on average age?

13. What is the name of the provider that has the highest total charge?

14. What is the name of the provider that has the least total charge for teenage male on average?

15. Create a season (Spring, Summer, Fall, Winter) variable. Calculate the length of stays by season.  Which season has the longest length of stays on average?

16. On average, how much a 20 year-old male get charged for staying 1 day in the Fall season?

17. Write a paragraph to summarize the section and give your comments on the results. You could do some other calculations to support your points. 

-------

## Example 1

Continue with the data from part I. 

1. Provides at least 10 meaningful plots. Comments on the plots. All plots should have title, caption, appropriate labels on x and y-axis

2. Make an animation plot. 

3. Write a paragraph to summarize the section and give your comments on the results. 

-------

## Example 2

Continue with the data from part I. Use the follows as the target and input variables: 

*Target Variable*: Create the target variable taking value of 

  - `low` if the total charge of a patient (`tot`) is smaller than the median of the total charge, and

  - `high` otherwise. 

*Input Variables*:

  - "provider","moa","mod","admtype","campus", 'los','diag_adm'
  
-------

1. Use `filter` function to filter out rows where `raceethn==''` or `admtype==''`. Make sure all the categorical variables are factor, numeric variables are numeric. Set Training : Testing Split = 10 : 90 

2. Train a decision tree using `rpart`.  Plot the decision tree. Plot the variable importance ranked by the tree. 

3. Using caret for this question. Set `Training Control` to be: Use Cross-Validation of 5 folds across all models.  Train & tune at least 2 different models (i.e. two different values for `method=` in the train function of caret).  Plot the hyper-parameter tuning plots for each model. 

4. Plot the comparison of the models in 3. 

5. What is your final selection for the model? Test the accuracy of your final model on the test data. 

6. Create another `target` variable (binary), decide the input variables and redo 1 to 5. 

7. Write a paragraph to summarize the section and give your comments on the results. 

-------
