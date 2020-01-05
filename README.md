# JAVACHRISTMASTASK
# Engineering 50 Christmas Task

## Intellij and Java 13

## Methodology
All codes were tested and documented under the 'Testing' header. Each code was tested, and solutions to the error had to be noted. The test was repeated until the test returned the correct output. Every change, along with it's respective output was documented under the 'Changes' header. 

#### Testing
1 True should be returned for the following code: divisbleBy(4,2).
- Output before changes - false
- Output after change - true

Problems:
- Did not return 'true'

2 The following code should return false: divisbleBy(3,2).
- Output before change - false

Problems:
- n/a

3 The code - fizzBuzzGenerator(1,15) - should return ["1","2","Fizz","4","Buzz","Fizz","7","8","Fizz","Buzz","11","Fizz","13","14","FizzBuzz"].
Output before changes: [1, FizzBuzz, 3, 4, FizzBuzz, 6, FizzBuzz, FizzBuzz, 9, 10, FizzBuzz, FizzBuzz, 13, FizzBuzz]
Output after change 1: [1, 2, FizzBuzz, 4, FizzBuzz, FizzBuzz, 7, 8, FizzBuzz, FizzBuzz, 11, FizzBuzz, 13, 14]
Output after change 2: [1, 2, FizzBuzz, 4, FizzBuzz, FizzBuzz, 7, 8, FizzBuzz, FizzBuzz, 11, FizzBuzz, 13, 14, FizzBuzz]
Output after change 3: [1, 2, Fizz, 4, Buz, Fizz, 7, 8, Fizz, Buz, 11, Fizz, 13, 14, FizzBuzz]
Output after change 5: [1, 2, Fizz, 4, Buzz, Fizz, 7, 8, Fizz, Buzz, 11, Fizz, 13, 14, FizzBuzz]

Problems:
1.  The code only returned 14 values instead of 15
2. 'FizzBuzz' triggered at the wrong place
3. 'Buzz' did not trigger
4.  Incorrect case in the code at '12', should be 'Buzz' instead of 'buzz'
5.  Wrong spelling for 'Buz', it should be "Buzz"

#### Changes
1. For 1.1 and 3.2: At FizzBuzzGenerator > divisibleBy() return numerator % Denominator == 2; to return numerator % Denominator == 0;
2. For 3.1:  At FizzBuzzGenerator > FizzBuzz() for (int i = startNumber; i <endNumber ; i++) { to for (int i = startNumber; i <= endNumber ; i++) {
3. For 3.3:  At FizzBuzzGenerator > FizzBuzz() if(divisibleBy(i, 3) || divisibleBy(i, 5)) fizzBuzzList.add("FizzBuzz"); to if(divisibleBy(i, 3) && divisibleBy(i, 5)) fizzBuzzList.add("FizzBuzz");
4. For 3.5: At FizzBuzzGenerator > FizzBuzz() else if (divisibleBy(i, 5)) fizzBuzzList.add("Buz"); to else if (divisibleBy(i, 5)) fizzBuzzList.add("Buzz");
