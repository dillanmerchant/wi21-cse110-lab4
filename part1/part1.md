1. Line 11 will print the length of <code>prices</code> because <code>i</code> is initialized with <code>var</code>. This means that the position of initialization does not matter, it can go in and out of code blocks.
2. Line 12 will print the discounted price of the last price in the <code>prices</code> array because even though it is in a code block, the <code>var</code> initialization allows it to travel outside of it. The discounted price was set to: current price * (1 - the discount)
3. Line 13 will have that same price in line 12, but rounded to the proper decimal points for a price (2 decimal points) using the <code>Math.round()</code> operation. Once again, this is possible because of the <code>var</code> initialization allowing it to work even outside the code block.
4. The function will return <code>discounted</code>, and discounted will be equal to <code>[50,100,150]</code>. Explanation - this function iterates through an array of prices. Within the loop, it takes each price and applies the given discount on it and makes sure it rounds the value into a valid currency value. The new prices are then pushed into a "discounted" array. This array of discounted prices is then returned.

&NewLine;
&NewLine;

5. At line 11, there will be a reference error because <code>i</code> is initialized with <code>let</code> in another code block. The scope does not reach outside the code block with the <code>let</code> initialization. Therefore, it will say the variable <code>i</code> is not defined.
6. At line 12, there will be a reference error because <code>discountedPrice</code> is initialized with <code>let</code> in another code block. The scope does not reach outside the code block with the <code>let</code> initialization. Therefore, it will say the variable <code>discountedPrice</code> is not defined.
7. At line 13, the last price in the <code>prices</code> array with the discount and rounding will be printed. Although it was initialized with <code>let</code>, it is not in another separate code block; thus, there is no error.
8. If line 11 and 12 are still there, this function will not run because of the variable scope errors. However, if they were removed, <code>[50,100,150]</code> would be returned because it is returning <code>discounted</code>, a variable initialized with <code>let</code>, but still in the same code block. Therefore, it will be initialized, then manipulated in another code block (in this case the for loop), and go back to the other code block to be returned.

&NewLine;
&NewLine;

9. At line 11, there will be a reference error because <code>i</code> is initialized with <code>let</code> in another code block. The scope does not reach outside the code block with the <code>let</code> initialization. Therefore, it will say the variable <code>i</code> is not defined.
10. At line 12, there will be a reference error because <code>discountedPrice</code> is initialized with <code>const</code> in another code block. The scope does not reach outside the code block with the <code>const</code> initialization. Therefore, it will say the variable <code>discountedPrice</code> is not defined.
11. At line 13, an error will occur regarding the type of initialization the <code>finalPrice</code> variable received, the <code>const</code> initialization. When a variable is initialized with <code>const</code>, that means that variables value cannot be updated. In the for loop, we see that the <code>finalPrice</code> variable is being chnaged after every iteration, thus creating the error of assigning to a constant variable.
12. If <code>discountPrices([100,200,300],.5)</code> is attempted, we see the initialization of both the <code>discounted</code> array and <code>finalPrice</code> variable with <code>const</code>. In the for loop, we are trying to update the <code>finalPrice</code> which will cause an error due to not being assign to a <code>const</code> variable. However, these variables must be altered in order for the function to behave properly. Therefore, the function will not return the discounted prices or anything in general besides an error.

&NewLine;
&NewLine;

13.
  * A. student.name
  * B. student['Grad Year']
  * C. student.greeting()
  * D. student['Favorite Teacher'].name
  * E. student.courseload[0]
  
&NewLine;
&NewLine;
  
14.
  * A. '3' + 2 = 32 --- this is because the addition sign will be used as concatenation in the string sense. The 2 is concatenated to the '3' string
  * B. '3' - 2 = 1 --- the subtraction sign will yield an automatic number conversion. The '3' will become a number and then it will be subtracted by 2
  * C. 3 + null = 3 --- the addition sign will be used for arithmetic because of the number 3 and the null will be converted to its numeric value 0, so it will be 3 + 0
  * D. '3' + null = 3null --- similar to a), the addition sign will be used for concatenation due to the '3' string. The word null will be concatenated to the already existing '3' string
  * E. true + 3 = 4 --- the addition sign will be arithmetic so it will convert true to its numeric boolean value 1 and add it to the existing 3
  * F. false + null = 0 --- the addition sign will be used for arithemtic so the number conversions for both of these would result in 0. Therefore, 0 + 0 = 0
  * G. "3" + undefined = 3undefined --- because there is a string, the addition sign will be used for concatenation. The word "undefined" will be concatenated to the existing "3" string
  * H. "3" - undefined = NaN --- the subtraction sign yields an automatic number conversion; the "3" is converted to 3 and the undefined is converted to NaN which results in the answer being NaN
15.
  * A. '2' > 1 is true --- the '>' comparison operator will have the '2' convert into a number. Therefore, 2 is greater than 1 so it will return true
  * B. '2' < '12' is false --- When comparing strings, we must follow the "dictionary" order. In this case, '2' is greater than '12' because '12' starts with a '1' which is less than '2'. Therefore, it is false
  * C. 2 == '2' is true --- the '==' operator allows for datatype conversion so the '2' string will be converted into a number. Therefore, 2 is equal to 2 so it will return true
  * D. 2 === '2' is false --- the '===' is strictly an equality operator and does not allow any conversions in datatype. Therefore, the string '2' in not equal to the number 2 and will return false
  * E. true == 2 is false --- the '==' operator allows for datatype conversion so the true will become a 1 after the boolean to number conversion. 1 is not equal to 2 so it would return false
  * F. true === Boolean(2) is true --- the '===' is a strict equality operator and will not automatically do any datatype conversions. However, in this case the conversion in explicitly shown so the 2 will be converted into a boolean. Since 2 is not 0, it will be converted into true. True is equal to true so it would return true
16. In Javascript, the <code>==</code> operator is used for comparing two variables, but in the process of comparing it ignores the datatypes of each variable and will most likely perform a type conversion. On the other hand, the <code>===</code> operator is used to compare two variables while checking the datatypes of each value as well.

&NewLine;
&NewLine;

17. The console will log 'How are you?'. Explanation - This code snippet shows an if, else if, else statement so we must go through all the conditions. First, we are  testing <code>2 == true</code>. Since it is the <code>==</code> operator, the datatypes are not checked and the true will be converted to a 1. Thus, 2 is not equal to 1 so it will continue on to the next condition. The next condition is simply <code>2</code>. Since it is expecting a boolean value, there will be a type conversion on 2 to a boolean. Since 2 is not 0 (false), it will convert to true which will allow it to enter the statement within that condition - <code>console.log('How are you?');</code>. In these type of if statements, it will skip the rest of the conditions if it enters one. Thus, this will have us reach the end the code snippet.

&NewLine;
&NewLine;

18. Can be found under part1-question18.js

&NewLine;
&NewLine;

19. With the following function <code>modifyArray</code> and parameters <code>([1,2,3], doSomething)</code>, we can walk through the program to get a result. First we create a <code>newArr</code> that is empty. Then we enter the for loop and we are pushing into the <code>newArr</code>. In this push, we are calling the callback method which is <code>doSomething</code> and it takes in two parameters: <code>num</code> which is passed in by <code>array[i]</code> and another callback which is passed in with a written function that takes a parameter <code>x</code>. So, we call the <code>doSomething</code> method with the first number in the array originally passed in - 1 and add it by 2. That value is then returned back to the written function where it now will return that value multiplied by 2. Then we take that value, which should be 2(x+2) at this point, and push it into <code>newArr</code>. We then repeat for the rest of the number in the original array passed in. This would reuslt in <code>newArr</code> being <code>[6,8,10]</code> and <code>newArr</code> is then returned.

&NewLine;
&NewLine;

20. Can be found under part1-question20.js

&NewLine;
&NewLine;

21. The output of this code should these numbers logged in this order, each with a new line: 1,4,3,2. This is because as soon as the function starts, the console logs 1. Then, there are setTimeouts for both the loggings of the numbers 2 and 3 so they enter their own event cycle. Since 4 is not a part of that event cycle and instead with the number 1, the number 4 will be logged next. We can then enter the next event cycle and see that the logging of 3 has no delay so it will log next. Finally, the logging of 2 will occur after a 1000 millisecond delay. This is the explanation behind the ordering of the loggings.

