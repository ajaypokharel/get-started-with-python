## Python List, Tuple, and Set Problems

***Note: This will contain a mix of problems I have created with the problems on platform such as HackerRank. If you do not have an account, I would recommend making one.***

1. What is the difference between a list, tuple, and set in Python? Think of an example where you might use each of these.

2. Look at the following program. What does this program print?

   ```python
   temp_list = []
   
   for item in range(25):
       if item % 2 == 0:
           temp_list.append(item)
   
   print(temp_list)
   
   ```

3. The code snippets below have bugs in them. You task is to debug, find, and fix the bug. Debugging is one of the most essential skills for a programmer. If you cannot find the bugs just looking at the code below, run the programs in a python environment (script/shell) and find the bugs.

   * Program 1: The program below needs to check the letter stored in the list `letter_list` match the letters stored in the string variable `letter_str`. It should print `True` for every matching letter, and  `False` if any letter do not match.

     Example1: `letter_list = ['H', 'E', 'L', 'P']`, `letter_str = 'HELP'`. This prints `True, True, True, True`. 

     Example2: `letter_list = ['h', 'i']`, `letter_str = 'hy'`. This prints `True, False`.

     ```python
     """
     Find the bug and fix it
     """
     
     letter_list = ['P', 'Y', 'T', 'H']
     letter_str = 'PYTH'
     
     if letter_list == letter_str:
         print('True')
     else:
         print('False')
     ```

   * Program 2:  The program needs to update the `lang` data type with few more programming languages `Java, JavaScript, Kotlin`.

     ```python
     lang = ('Python', 'C')
     to_be_added = ('Java', 'JavaScript', 'Kotlin')
     
     for item in to_be_added:	# this loops through to_be_added -> Java -> JavaScript -> Kotlin
         lang.append(item)
     
     print(lang)
     ```

   * Program 3: There is a bug in the program below. Find it and think about the reason the program does not work.

     ```python
     my_set = set()
     
     my_set.update([2, 3, 4, 9])	# this appends 2, 3, 4, 9 to my_set.
     
     my_set[2] = 7
     ```

   * Program 4:  The program needs to count the number of times a number appears in a given list. Any decimal, integer or complex number inside a string parenthesis is also considered a number for the sake of this problem. `'3', '3.14'` are also numbers. Our program does not work properly. Find the bug and fix it!

     ```python
     """
     Find and fix the bug!
     """
     
     my_list = ['P', 't', 2, 'h', 92, '8', '2.345', 'hi']
     count = 0
     
     for item in my_list:
         if isinstance(item, int):
             count += 1
     
      print(count)
     ```

4. This is a Hackerrank problem: [Tuples](https://www.hackerrank.com/challenges/python-tuples/problem?isFullScreen=true)

5. This is a Hackerrank problem: [Lists](https://www.hackerrank.com/challenges/python-lists/problem?isFullScreen=true)

6. This is a Hackerrank problem: [Sets](https://www.hackerrank.com/challenges/py-introduction-to-sets/problem?isFullScreen=true)

7. This is a Hackerrank problem: [Set .add](https://www.hackerrank.com/challenges/py-set-add/problem?isFullScreen=true)

8. What is tuple unpacking?

9. Examine the code below and write what the print function will print:

   ```python
   new_tup = (2, 3, 6, 12, 99)
   
   x, *y, z = new_tup
   
   print(x)
   print(z)
   ```

10. What is wrong with the following attempt in initializing a tuple with a single element. How would you fix it?

    ```python
    new_tup = ('python')
    ```

    
