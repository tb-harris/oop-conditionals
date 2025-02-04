# Booleans and Conditionals - Pracitce Exercises
Don't forget to write your code in a `main()` method - in 
IntelliJ you can just type "main" inside of the class definition
and it will autocomplete.

## CanDrive
* Write a program that tells a user whether they are old enough to drive.
* Command Line Arguments: `<age>`
* Output: "You can drive" or "You can't drive"

## LeapYear
* Write a program that tells a user whether the given year is a leap year.
* Command Line Arguments: `<year>`
* Output: "___ is a leap year" or "___ is not a leap year"
* Hint: Leap years occur every four years. Look back at the even vs odd example from the w3schools reading.

## VowelChecker
* Write a program that tells a user whether a letter is a vowel or not.
* Command Line Arguments: `<letter>`
* Output: "Vowel" or "Consonant"

## CanRegister
* Write a program that tells the user whether they are eligible to register to vote. To pre-register to vote in NY, you must be a US citizen and at least 16 years old.
* Command Line Arguments: `<age>` `<isCitizen>`
    * The second argument should be `true` if the user is a citizen and `false` if they are not.
* Hint: Use the `&&` operator to make sure that both conditions are met.

## GoldfishCare
* A goldfish needs temperatures between 20-23 degrees Celsius and a tank size of at least 20 gallons. Write a program that tells the user whether they are ready to get a goldfish based on their aquarium setup.
* Command Line Arguments: `<tankSize> <temperature>`
* Output: "You are ready for a goldfish!" or "You need to make some changes before getting a goldfish."
* Hint: Use the `&&` operator to make sure that all conditions are met. You will need to use three comparisons in total.

## AnimalCare
* Research another fish, reptile, or other animal of your choice. Write a program similar to GoldfishCare that tells the user whether they are ready to get that specific animal.
* Document your program's required arguments in a comment at the top of your program.

# Bonus Problems
## LeapYear (Updated)
* The true rule for leap years is a little more complicated: if a year is not divisible by 100, it is NOT a leap year, unless it is also divisible by 400. For example, 1900 and 2100 are not leap years, but 2000 is. Update your program to account for this rule.

## RocketLaunch
**Problem**
The following are a selection of the [Atlas V Launch Weather Criteria](https://www.nasa.gov/wp-content/uploads/2018/04/633165main_atlas-5-weather.pdf?emrc=ea1836):

1. Do not launch if the wind at the launch pad exceeds 33 knots (38 mph).
2. Do not launch if the ceiling is less than 6,000 feet or the visability is less than four nautical miles.
3. Do not launch through or within five to 10 miles of cumulus clouds with tops that extend into freezing temperatures.
4. Do not launch within 10 nautical miles of the edge of a thunderstorm that is producing lightning for 30 minutes after the last lightning is observed.
5. Do not launch for 30 minutes after lightning is observed within 10 nautical miles of the launch pad or the flight path unless specified conditions can be met.

Write a program that takes in all of the necessary weather readings (for example, wind speed, cloud ceiling, visability, etc). For conditions that involve time, make sure to take in the time of the last observed lightning strike. **Document the command line arguments for your program in a comment at the top.**

Your program should output a message for each condition showing whether it is met or not (see example). Then the program should output either "Go" or "No go". A delayed launch should output "No go".

**Hint:** Create boolean variables for each of the five conditions. You can then use each variables in the if statement for the conditions, and then re-use them in the final if statement.

**Example Output**
```
✅︎ Condition 1
❌ Condition 2
✅︎ Condition 3
✅︎ Condition 4
✅︎ Condition 5

No go.
```

## FindMyDean
* **Use a switch statement for this program!** Write a program that takes the user's grade as an integer argument. If the user in 6th through 12th grade, it should output their [dean's name](https://www.riverdale.edu/about/whos-who-at-riverdale#h-middle-school-administrative-team). If the user gives an integer outside of that range, output "You do not have a dean".
* Command Line Arguments: `<grade>`

## CanDrive (Updated)
Rewrite the CanDrive program **using the ternary operator.** You should be able to replace the entire if-else statement with a single line of code.