# Random-Password-Generator-Using-Python
This is a Python script that generates a random password based on user-defined length. 
<br>
The password is created using a combination of uppercase and lowercase letters, numbers, and special characters.
<br>
## Code Breakdown
<br>
import random: Imports Python's built-in random module, which allows for generating random values and selecting random items from a sequence.<br>
characters = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!@#$%&*1234567890":<br>
This line defines a string called characters that contains:<br>
All lowercase letters (a-z).<br>
All uppercase letters (A-Z).<br>
Special characters (!@#$%&*).<br>
Numbers (0-9).<br>
The string characters serves as a pool from which characters can be randomly selected, making it ideal for tasks such as generating secure passwords, random keys, or tokens.<br>
<br><br>
length = int(input("Enter Password length: ")):<br>
input(): Prompts the user to enter the desired password length. The input is captured as a string by default.<br>
int(): Converts the user input from a string to an integer, which ensures that the length is a numeric value.<br>
length: Stores the length of the password entered by the user.<br>
Password = "":<br>
This initializes an empty string called Password. As the program loops to generate random characters, they will be appended to this string to form the final password.<br><br>

for i in range(length)::<br>
This line creates a loop that will iterate length times, where length is the number of characters the user specified for the password. The loop variable i is not used within the loop, but it helps control the number of iterations.<br>
Password += random.choice(characters):<br>
random.choice(characters): This function randomly selects one character from the characters string during each iteration of the loop.<br>
Password += ...: This appends the randomly selected character to the existing Password string, gradually building the password character by character.<br>
print(Password):<br>
After the loop completes, this line prints the final randomly generated password to the console.<br>
