import random


# Get a random word from a list
word_list = ["stick","john","pencil","rubber","glove","quick","brown","fox","jumps","over"
                     ,"lazy","dog","manner","house","food","brain","history","love","peace",
                      "object"] 


chosen_word = random.choice(word_list)
#print (chosen_word) #Test

#build a shell (list)
#print (len(chosen_word)) #Test
playerchoice = ['_' for i in range(len(chosen_word))]
print (playerchoice)

# inital setting
life = 10
print ('Life remains: '+ str(life))

#Start while loop
while life >0:
    #Bingo
    if sum(a == '_' for a in playerchoice) == 0:
        print("Bingo!")
        break
    else:
    #input
        guess = str(input('Input a letter: '))
    # >1 letter
        if len(guess) > 1:
            print ('Only one letter')
        else:
            #check letter in the chosen_word
            for i in range(len(chosen_word)):
                if guess == chosen_word[i]:
                    playerchoice[i]=guess       
    
    #show guess's result
    life = life - 1
    print (playerchoice)
    print ('Life remains: '+ str(life) + ' . ')
    
    #No life
    if life == 0:
        print('Gameover! ')
