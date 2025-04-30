1. Since we declared the value of i as a var, it will be accessible from the entire function scope.  This goes through the length of the list, reach a value of 3 before it fails the for loop condition and breaks the loop.  Thus, the console will log its final value of ```3```.
2. Since discountedPrice is declared with var, its value is accessible throughout the function scope.  With the loop, the discountedPrice value is redeclared to the discounted price for each value in price.  Finally, it ends with the last value being 300 discounted to 150.  This the console logs ```150```.
3. This declaration of finalPrice may only be once at the start as 0, but its scope with var being the function lets it be updated.  It is updated to the value of discountedPrice rounded to 2 decimal places so it takes the last such value of discountedPrice which is 150.  Thus the console logs ```150```
4. This would return the a new list of all the updated values after updating the price with the discounts.  In our case, we would get ```[50,100,150]```
5. Since we declared i with let at the for loop, its scope is limited to the for loop.  Since the console log happens outside the for loop, it cannot find this value of i and thus errors.
6. Since we declared discountedPrice with let in the for loop, its scope is limited to the for loop.  Since the console log happens outside the for loop, it cannot find this value of discountedPrice and thus errors.
7. Even though final price was declared with let, it was declared at the start of the function and thus has a function scope.  So it would work similarly to var and the for loop would update it.  finalPrice would take the final discounted down to 2 decimal value having the console log ```150```
8. Even though discounted was declared with let, it was declared at the start of the function and thus has a function scope.  So it would work similarly to var and the for loop would update it.  discounted would take all the final prices having the return value be the list ```[50,100,150]```
9. Since we declared i with let at the for loop, its scope is limited to the for loop.  Since the console log happens outside the for loop, it cannot find this value of i and thus errors.
10. Length declared as a const would hold the value for the length of the prices list that was passed in of 3.  It would never change due to the const value and the console would log ```3```
11. Even though the list is getting values added to it is const, it still can get values pushed to it as const just prevents us from reinitializing the declared variable not changing it though the list add function.  Also, even though discountedPrice is a const since we are redeclaring it each time, it makes a completely new variable each time and thus its value does change.  This gives us the return value of ```[50,100,150]```
12. Here are the following notations
    1.  To access the name of student, we would call ```student.name```
    2.  To acces the value of the Grad Year, we would call ```student["Grad Year"]```
    3.  To get the name property of the object in the Favorite Teacher property in student, we would call ```student["Favorite Teacher"].name```
    4.  To get the  index zero in the array of the courseLoad property of the student object, we would call ```student.courseLoad[0]```
13. Here are the outputs and explanation why that was given
    1.  '3'+2 gives us '32' as it converts 2 to a string and does the join operation to get the new string
    2.  '3'-2 gives us 1 as - needs numbers so it converts '3' to a number and does the operation and gets 1
    3.  3 + null gives us 3 as null is treaded as a number of 0 giving us 3
    4.  '3' + null gives us '3null' as it converts null to the string 'null' and applies the string concatenation to give us '3null'
    5.  true + 3 gives us 4 as true is converted to the number 1 and the add operation gives us 4
    6.  false + null gives us 0 as false converts to the number 0 just like null which lets us do the add operation to give us 0
    7.  '3' + undefined gives us '3undefined' as it converts undefined to the string 'undefined' and applies the string concatenation to give us '3undefined'
    8.  '3'-undefined errors giving us NaN as '3' may be converted to a number but undefined cannot be causig this error
14. Here are the outputs and explanation why that was given
    1.  '2' > 1 gives us true as '2' is converted to number 2 and 2 is bigger than 1 giving us true
    2.  '2' < '12' gives us false.  Though 2 is less than 12, since both values here are strings we are comparing the lexilogical order which has '12' before '2' so its value is smaller giving us false
    3.  2 == '2' gives us true as the string '2' is converted to the number which converts it to true
    4.  2 === '2' gives us false as the === checks for type matching too which here does not work, thus it is false
    5.  true == 2 is false as true's integer value is 1 which is not equal to 2
    6.  true == Boolean(2) is true because Boolean(2) converts 2 to true which is because 2 is a nonzero value.  Since both values are now a boolean true, this returns true.
15. == is a loose equality while === is a strict equality.  == does comparsions after doing any needed type conversions while === does not do this step.  This is the main difference.
16. Added Code to the JavaScript file
17. When we run this code, we fist call modifyArray with the parameters of [1,2,3] and doSomething as the callback.  We then iterate though the array and we update the values in the array by applying the function of the callback.  doSomething (which is our callback) doubles the number value.  Thus, at the end of this, we would get the array of all the values but doubled giving us ```[2,4,6]```
18. Added code to the JavaScript file
19. This code would print 1 first and then set a timeout of one second for printing 2 and then one of zero milliseconds for 3 and then prints four.  So we then print four and the zero second timeout ended so we print 3.  After one second, we print the value of 2.  This gives us the final output of ```1 \n 4 \n 3 \n 2```.  (The \n is a line break)