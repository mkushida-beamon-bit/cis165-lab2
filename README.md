## CIS-165 Lab 2
# Course Information
# Course section: [CIS-165-W099]

## Lab: Lab 2
# Programs: sum.cpp and mpg.cpp

## Initial Plans
# Plan for sum.cpp
I need to store the values 50 and 100 in variables. I then add the two values together and store the result in a variable named total. Then I will display the value of total with a clear label.

# Plan for mpg.cpp
I need to store 312 miles and 16 gallons in variables. I will divide the number of miles by the number of gallons and store the result in a variable. I will use a data type that can preserve the fractional result and then display the result with the MPG units.

## How to Compile and Run
#sum.cpp
To compile the program using g++, use:
g++ -std=c++17 -Wall -Wextra sum.cpp -o sum

## mpg.cpp
To compile the program using g++, use:
g++ -std=c++17 -Wall -Wextra mpg.cpp -o mpg

## Testing
Before each test, I calculated the expected result myself and then compared it with the actual program output.

Program	Values used	Expected result before running	Actual output	Match or fix
sum.cpp — assigned values	50 and 100	150	Total: 150	Match
sum.cpp — changed values	25 and 75	100	Total: 100	Match
mpg.cpp — assigned values	312 miles; 16 gallons	19.5 MPG	Miles per gallon: 19.5 MPG	Match
mpg.cpp — changed values	100 miles; 8 gallons	12.5 MPG	Miles per gallon: 12.5 MPG	Match

After completing the changed-value tests, I restored the originally assigned values in both programs and reran them. The final versions of sum.cpp and mpg.cpp use the original assigned values.

## Code Explanation
# sum.cpp
In sum.cpp, I first store 50 and 100 in the variables, first_number and second_number respectively. Then I add the two values together. The result is stored in the variable named total, which is 150. I store the calculation in total before printing because it lets the program calculate the answer first and then print the result stored in the variable and makes it easier for someone to read and understand the code.
# mpg.cpp
In mpg.cpp, I calculate MPG by dividing miles by gallons. I used 312 miles and 16 gallons for the assigned values. I chose the double data type because MPG can have a fractional answer, and 312 divided by 16 equals 19.5 MPG. If both values were integers, C++ would perform integer division and drop the decimal portion. For my changed-value test, I used 100 miles and 8 gallons, so I expected 12.5 MPG, and the program displayed 12.5.
## Changed MPG Test
For my changed MPG test, I used 100 miles and 8 gallons. Before running the program, I calculated the expected result by dividing the miles by the gallons: 100 ÷ 8 = 12.5 MPG. I entered these values into the miles and gallons variables. The program then divided miles by gallons and stored the result in the mpg variable. When I ran the program, it displayed 12.5 MPG, which matched my expected result.
