# Antonym-Synonym-game---Covid-work
Code for antonym and synonym pair

import random
score = 0

word_list_1 = ["hot","summer", "hard", "dry", "simple", "light", "weak", 
               "male", "sad", "win", "small", "ignore", "buy", "succeed", 
               "reject", "prevent", "exclude"]

word_list_2 = ["cold","winter", "soft", "wet", "complex", "heavy", "strong", 
               "female", "happy", "lose", "big", "pay attention", "sell", 
               "fail", "accept", "allow", "include"]

lengthList_1 = len(word_list_1);
lengthList_2 = len(word_list_2);

random_index = random.randint(0,lengthList_1-1)
pair_word01 = word_list_1[random_index]
pair_word02 = word_list_2[random_index]

random_index2 = random_index
while random_index2 == random_index:
  random_index2 = random.randint(0,lengthList_1-1)
question_word01 = word_list_1[random_index2]

 

print(pair_word01 + " is to " + pair_word02 + " as " + 
      question_word01 + " is to...")


the_answer = word_list_2[random_index2]

user_answer = str(input("Enter the answer: "))
if user_answer == the_answer:
    print("Correct, Well done")
else:
    print("Wrong!")
    print("The right answer is: " + the_answer)
    
    
    
# EXTENSION TASK
The extension code in pseudocode:
Firstly, i will address the file in my code with  KEY, SYNONYM_LIST, ANTONYM_LIST. 
which will allow me to access the file with my code. i will then use the R+ feature to read the file and then access its contents. 
i will like with my code then place them all in questions ensuring that i dont repeat any of them.
again i will use a score = score + 1 everytime they get the question rightand print the final score. 
The only problem will be assigning the indexes to each antonym and synonym pair in the text file as my code exploits the fact that the synonym and antonym pair are in the same indexes in 2 different lists. 

And so for my code, i will also try to emulate the same idea. 
    
