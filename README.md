# Password-Strngth-checker
this porgram checksthe strength of an inputed password


# To ask user for input
passwordInput= input("Enter your password: ")

# Check for the length
if len(passwordInput) > 8:
    print("Strong")
else:
    print("Weak")

# check for uppercase
has_upper= any(char.isupper() for char in passwordInput)

if has_upper:
    print("Strong")
else:
    print("Weak")

# check for special charcters
special= "!@#$%^&*()"

has_special= any(char in special for char in passwordInput)

if has_special:
    print("Strong")
else:
    print("Weak")

