# PA#1
### Name: AGAPITO, Catalino D.R.
### Section: 2ECE-C
### Date Submitted: August 27, 2026

In this Program Assignment, three different problems were asked. Each problem has its own function for performing a specific task.

# Problem 1: Word Rotation Problem

In this problem, you are asked to rotate a given word by moving its first letter to the end. For example, the word "python" should become "npytho". In order to create a function that rotates a word by moving its first character to the end, the following code syntax is used.

First, the program asks for the text to be rotated using the 'input()' syntax. 
The input is stored in 'word' before being processed by the rotate_word() function.
````
def rotate_word(text): 
return text[1:] + text[0]
word = input("Enter text: ") #asks the user to eanter a word to rotated
print(rotate_word(word)) #prints the result
````


# Problem 2: Username Builder Problem

In Problem 2, you are asked to create a function that builds a username from a user's first and last name. The username should be in lowercase format with a dot (.) separating the 
first and last names. For example, "Catalino" and "Agapito" become 
"catalino.agapito".

In order to create a function that builds a username from first and last names, 
The following code syntaxes are used.

First, the program asks for the user's first name using the 'input()' syntax. 
The input is stored into 'first' before being processed. Then, the program asks 
for the user's last name using another 'input()' syntax, stored into 'last'.

````
def make_username(first_name, last_name):
    first_name = first_name.lower().replace(" ", "") 
    last_name = last_name.lower().replace(" ", "") 
    return first_name + "." + last_name

first = input("enter first name: ") #asks the user for their first name
last = input("enter last name: ")  #asks the user for their first name
username = make_username(first, last) #constructs the username
print(username) #prints the username
````

# Problem 3: Bookend Swap Problem

In Problem 3, you are asked to create a function that swaps the first and last elements of a list. This is called "bookend swapping" because the elements at the ends (bookends) are 
exchanged while the middle elements remain in their original order. 
For example, ["book", "item", "pencil"] becomes ["pencil", "item", "book"].

In order to create a function that swaps the bookends of a list, the following 
Code syntaxes are used.

First, the program asks for items using the 'input()' syntax. The input is 
stored into 'items' before being processed.

````
def swap_bookends(items):
    first, *middle, last = items
    return [last] + middle + [first]
items = input("Enter items: ") #asks the user to enter items
initems = items.split()
swap = swap_bookends(initems)
print(swap)
````
