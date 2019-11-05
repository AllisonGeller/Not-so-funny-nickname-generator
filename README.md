# not-so-funny-nickname-generator
#Your jokes aren't as funny as you think they are.

import sys, random

print ('Welcome to the Not-So-Goofy Name Picker')
print ("Those nicknames aren't as funny as you think they are")

first  = ('woof', 'yikes', 'uh-oh', 'no no', 'oh god why', 'is this really necessary', 'dude come on', 'seriously stop', 'this isnt even funny anymore', 'can you please cut this out?')

last = ('oh come on', 'this is totally funny', 'you love it', 'you know im just kidding', 'i love you man', 'dont get mad!', 'its a joke!', 'you would do it to me!', 'im sorry!')

while True:
    firstname = random.choice(first)
    
    lastname = random.choice(last)
    
    print("\n\n")
    print("{}, {}".format(firstname, lastname), file=sys.stderr)
    print("\n\n")
    
    try_again = input("\n\nTry Again? (Press enter else n to quit)\n ")
    if try_again.lower() == "n":
        break
        
input("\nPress enter to exit.")
