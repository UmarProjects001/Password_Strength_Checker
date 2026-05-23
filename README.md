Password=input("Enter your Password: ")
score=0
if len(Password)>=8:
    print("Password is of good length")
    score+=1
else:
    print("Password is too short")
special_chars = "@#$!%&*?+=_- "
if any(char in special_chars for char in Password):
    print("Password Contains special characters")
    score+=1
else:
    print("Password does not contain special characters")
if any (char.isupper() for char in Password):
    print("Password contains Upper case letters")
    score+=1
else:
    print("Password does not contain Upper case letters")
if any(char.isdigit() for char in Password):
    print("Password has numbers")
    score+=1
else:
    print("Password does'nt has numbers")
print("Your password strenght on a 4 scale is:",score)
if score >=3:
  print("Your password is strong")
elif score <=1
print("Your password is weak")
else:
print("Your password is of medium strength")
