# 🏆 Hackerrank:Runner-Up Score Finder in Python

## 🎯 AIM:
To write a Python program that takes a list of scores from participants and finds the **runner-up score** (i.e., the second-highest score), eliminating any duplicates.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create a variable `n` and get its value from the user (number of participants)
3. Read the list of `n` scores from the user using `input().split()` and convert them to integers
4. Store the scores in a list
5. Use `set()` to remove any duplicate scores
6. Convert the set back to a list and sort it in ascending order
7. Print the second-last element of the sorted list (i.e., the runner-up score)
8. **Stop**

---

## 💻 PROGRAM:
```
def find_runner_up(scores):
   
    unique_scores = set(scores)
    sorted_scores = sorted(unique_scores, reverse=True)

    if len(sorted_scores) > 1:
        return sorted_scores[1]
    else:
        return None  # Return None if there is no runner-up

scores = [45, 67, 89, 89, 91, 67, 72, 91]

runner_up = find_runner_up(scores)

if runner_up is not None:
    print(f"The runner-up score is: {runner_up}")
else:
    print("There is no runner-up score.")
```
## OUTPUT:
```
           Input                                              Result
 [45, 67, 89, 89, 91, 67, 72, 91]                [45, 67, 89, 89, 91, 67, 72, 91]
````
## RESULT:
The program was successful.
