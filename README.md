# PA1
In this Program Assignment, three different problems were asked. Each problem has its own function for performing a specific task.

<b> Problem 1: Word Rotation Problem

In this problem, you are asked to rotate a given word by moving its first letter to the end. For example, the word "python" should become "npytho". In order to create a function that rotates a word by moving its first character to the end, the following code syntax is used.

First, the program asks for the text to be rotated using the 'input()' syntax. 
The input is stored in 'word' before being processed by the rotate_word() function.
````
def rotate_word(text):
return text[1:] + text[0]
word = input("Enter text: ")
print(rotate_word(word))
````
The result is then printed to the screen using the print() function.
