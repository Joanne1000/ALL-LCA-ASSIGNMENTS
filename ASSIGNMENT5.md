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
