# Word-guessing-game
import random

tries = 0

print "Welcome to the word game!"
print "\nI'm going to think of a word and you have to guess it!"
print "\nGuess which letters are in the word, then you have to guess the whole thing!"
print "\nGood luck!"

WORDS = ("follow", "waking", "insane", "chilly", "massive", 
         "ancient", "zebra", "logical", "never", "nice")

word = random.choice(WORDS)

correct = word
length = len(word)
length = str(length)

guess = raw_input("The word is " + length + " letters long. Guess a letter!: ")

while tries < 5:
    for guess in word:
        if guess not in word:
            print "Sorry, try again."
        else:
            print "Good job! Guess another!"

    tries = tries + 1 #*

    if tries = 5:
        final = raw_input ("Try to guess the word!: ")

        if final = correct:
            print "Amazing! My word was ", word, "!"

        else:
            print "Sorry. My word was ", word, ". Better luck next time!"

raw_input("\n\nPress enter to exit")
