# Palindrom-Python
# Determines if users input word is a palindrome

def isPalindrome():
    string = str(raw_input('Enter a word: '))
    string1 = string[::-1]
    if string[0] == string[(len(string)-1)] and string[1:(len(string)-2)] == string1[1:(len(string)-2)]:
            print(string + ' is a palindrome.')
    else:
        print(string + ' is not a palindrome.')
isPalindrome()

# The [::-1] function is a slice that acts as a target assignment. 
# The syntax for this function is 'slice[start:stop:step]'
# In the instence of the palindrome code, I am telling the slice to
# not start nor stop at any given location in the string.
# This way, the entire string is always included.
# the step is -1 becasue this tells the slice to start at the end of 
# the string and work backwards by 1 increment each time.
# The slice will then return the entire string backwards.
