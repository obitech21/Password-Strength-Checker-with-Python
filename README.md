# Password-Strength-Checker-with-Python

# Introduction
In the world of cybersecurity, millions of breaches happen every year. Many of those breaches are due to users having 
weak passwords, or using the same password from multiple sites. Doing this only increases the risk of identity theft, 
and sensitive data being compromised.

Users should ensure that their passwords are strong and hard to guess in order to prevent losing any sensitive information
to any attackers. 

<br>
<br>
<br>


# Password Strength Checker Code

I first imported the required libraries for this project.

```python
import string
import getpass
import re
```

<br>
<br>
<br>

Then I added, "getpass" into the Python code which was used to encrypt the password when entered.
```python
password = getpass.getpass("Enter password: ")
```

<br>
<br>
<br>

After that, I created the requirements for the passwords.
```python
if len(password) < 10:
        print("This password is too short. Your password needs to be at least 10 characters long.")
        
elif not re.search("[A-Z]", password):
        print("Password needs at least one uppercase letter.")
        
elif not re.search("[a-z]", password):
        print("Password needs at least one lowercase letter.")
        
elif not re.search("[0-9]", password):
        print("Password needs at least one number.")
        
elif not re.search('[!@#$%^&*(),?":{}|<>]', password):
        print("Password needs at least one special character.")
        
else:
        print ("Password is good to go.")
```

<br>
<br>
<br>

The code will prompt the user to enter a password and inform the user on whether the passwords is strong or not.

I noticed that using "getpass" in Python code helped to encrypt the password. 

![1](https://github.com/obi298/Password-Strength-Checker-with-Python/assets/90945162/bdba1860-0c94-443a-bda4-06a8ac8dd22f)

<br>
<br>
<br>

When users enters a password that doesn't meet the requirements, the code will give suggestions on what they should add in their password.


![2](https://github.com/obi298/Password-Strength-Checker-with-Python/assets/90945162/829a9804-06b0-4df1-960b-e3de0f9970cf)

<br>
<br>
<br>

If a user enters a strong password that meets all the requirements, the code will say "Password is good to go."

![3](https://github.com/obi298/Password-Strength-Checker-with-Python/assets/90945162/093ccda2-e638-4ef8-8c66-1b37eb9783b4)

<br>
<br>
<br>

# Conclusion

This was a fun project and I learned more about using strings and adding encryption in Python. Organizations should advise employees to use strong passwords that contain a mix
of letters, numbers and special characters to reduce the likelihood of a security breach.











