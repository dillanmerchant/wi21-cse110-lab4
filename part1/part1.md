1. Line 11 will print the length of "prices" because "i" is initialized with var
2. Line 12 will print the discounted price of the last price in the prices array because even though it is in a code block, the var initialization allows it to travel outside of it. The discounted price was set to: current price * (1 - the discount)
3. Line 13 will have that same price in line 12, but rounded to the proper decimal points for a price (2 decimal points). Once again, this is possible because of the var initialization.
4. The function will return discounted, and discounted will be equal to [50,100,150]. Explanation - this function iterates through an array of prices. Within the loop, it takes each price and applies the given discount on it and makes sure it rounds the value into a valid currency value. The new prices are then pushed into a "discounted" array. This array of discounted prices is then returned.
5. At line 11, there will be a reference error because "i" is initialized with "let" in another code block. The scope does not reach and it will say it is not defined.
6. At line 12, there will be a reference error because "discountedPrice" is initialized with "let" in another code block. The scope does not reach and it will say it is not defined.
7. At line 13, the last price in the array with the discount and rounding accounted for will be printed. This is because although it was initialized with "let", it is not in another separate code block.
8. If line 11 and 12 are still there, this function will not run because of the variable scope errors. However, if they were removed, [50,100,150] would be returned because it is returning discounted, a variable initialized with "let", but still in the same code block. Therefore, it will be initialized, then manipulated in another code block (in this case the for loop), and go back to the other code block to be returned.
9.
10.
11.
12.
13.
a) student.name
b) student['Grad Year']
c) student.greeting()
d) student['Favorite Teacher'].name
e) student.courseload[0]
14.
a) '3' + 2 = 32; this is because the + sign will be used as concatenation in the string sense. The 2 is concatenated to the '3' string
b) '3' - 2 = 1; the - sign will yield an automatic number conversion. The '3' will become a number and then it will be subtracted by 2
c) 3 + null = 3; the + sign will be used for arithmetic because of the number 3 and the null will be converted to its numeric value 0, so it will be 3 + 0
d) '3' + null = 3null; similar to a), the + sign will be used for concatenation due to the '3' string. The word null will be concatenated to the already existing '3' string
e) true + 3 = 4; the + sign will be arithmetic so it will convert true to its numeric boolean value 1 and add it to the existing 3
f) false + null = 0; the + sign will be used for arithemtic so the number conversions for both of these would result in 0. Therefore, 0 + 0 = 0
g) "3" + undefined = 3undefined; because there is a string, the + sign will be used for concatenation. The word "undefined" will be concatenated to the existing "3" string
h) "3" - undefined = NaN; the - sign yields an automatic number conversion; the "3" is converted to 3 and the undefined is converted to NaN which results in the answer being NaN
15.
a)

