Input:
def check_string(s): 
    return s.isalnum()
# Example usage
s1 = "Hello123"
s2 = "Hello 123!" # contains space and special character
print(check_string(s1)) # True 
print(check_string(s2)) # False

Output:
True
False

INPUT:
import re
#Return a list containing every occurrence of "ai":

txt = "The rain in Spain"
x = re.findall("ai",txt)
print(x)

OUTPUT:
['ai', 'ai']

INPUT:
import re
#Check if the string starts with "The" and ends with "Spain":

txt = "The rain in Spain"
x = re.search("^The.*Spain$",txt)

if x:
    print("YES! We have a match!")
else:
    print("No match")

OUTPUT:
YES! We have a match!

INPUT:
import re

def check_string(s):
    pattern = "^[A-Za-z0-9]+$"  #^=start,$=end,+=one or more
    return bool(re.match(pattern,s))

#Example usage
s1 = "Hello123"
s2 = "Hello_123"  #contains underscore

print(check_string(s1)) #True
print(check_string(s2)) #False

OUTPUT:
True
False
