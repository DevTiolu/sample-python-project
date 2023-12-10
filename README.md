# sample-python-project

#A Python program to convert temperatures to and from Celsius and Fahrenheit.

#The centigrade to Fahrenheit conversion formula is: C = (5/9) * (F - 32) where C is Celsius and F is Fahrenheit.

#Prompt the user to input a temperature to be converted.

temp = input

#Extract the numerical part of the temperature and convert it to an integer

degree = int(temp[:-1])

#Extract the convention part of the temperature input (either 'C' or 'F')
i_convention = temp[-1]

#Check if the input convention is in uppercase 'C' (Celsius)
if i_convention.upper() == "C":
    # Convert the Celsius temperature to Fahrenheit
    result = int(round((9 * degree) / 5 + 32))
    o_convention = "Fahrenheit"  # Set the output convention as Fahrenheit
#Check if the input convention is in uppercase 'F' (Fahrenheit)
elif i_convention.upper() == "F":
    # Convert the Fahrenheit temperature to Celsius
    result = int(round((degree - 32) * 5 / 9))
    o_convention = "Celsius"  # Set the output convention as Celsius
else:
    # If the input convention is neither 'C' nor 'F', print an error message and exit the program
    print("Input proper convention.")
    quit()

#Display the converted temperature in the specified output convention
print("The temperature in", o_convention, "is", result, "degrees.") 

Sample Output:

Input the  temperature you like to convert? (e.g., 45F, 102C etc.) : 104f                                     
The temperature in Celsius is 40 degrees. 
Flowchart:

Flowchart: Python program to convert temperatures to and from celsius, fahrenheit

Python Code Editor:



Have another way to solve this solution? Contribute your code (and comments) through Disqus.

Previous: Write a Python program to find those numbers which are divisible by 7 and multiple of 5, between 1500 and 2700 (both included).
Next: Write a Python program to guess a number between 1 to 9.

What is the difficulty level of this exercise?

EASY MEDIUM HARD
Based on 3016 votes, average difficulty level of this exercise is Easy .
