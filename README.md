# Guess-A-Number
import random
number = random.randint(10, 20)

player_name = input("Hello, What's your name?")
number_of_guesses = 0
print('okay! '+ player_name+ ' Select  a number between 10 and 20:')

while number_of_guesses < 5:
    guess = int(input())
    number_of_guesses += 1
    if guess < number:
        print('Your guess is too low')
    if guess > number:
        print('Your guess is too high')
    if guess == number:
        break
if guess == number:
    print('You guessed the number in ' + (number_of_guesses) + ' tries!')
else:
    print('You did not guess the number, The number was ' + str(number))
