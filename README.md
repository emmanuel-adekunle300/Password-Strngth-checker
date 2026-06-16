# Password-Strngth-checker
this porgram checksthe strength of an inputed password


passwordInput= input("Enter your password: ")

if len(passwordInput) > 8:
    print("Strong")
else:
    print("Weak")

has_upper= any(char.isupper() for char in passwordInput)

if has_upper:
    print("Strong")
else:
    print("Weak")

special= "!@#$%^&*()"

has_special= any(char in special for char in passwordInput)

if has_special:
    print("Strong")
else:
    print("Weak")

