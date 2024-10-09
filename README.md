# Hunar-intern
import re

password = input("Enter your password : ")

if len(password) <8:
    print("Password must be atleast 8 character long. ")
elif not re.search("[A-Z]",password):
    print("Passowrd must contain atleast one upper case letter.")    
elif not re.search("[a-z]",password):
    print("Passowrd must contain atleast one lower case letter.")
elif not re.search("[0-9]",password):
    print("Passowrd must contain atleast one number.")
elif not re.search("[@,#,$,%,^,&,*]", password):
    print("Passowrd must contain atleast one special character.")
else:
    print("Password is strong")   
