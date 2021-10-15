# Login-system-MVP

This is a small project for practicing user authentication and login.

#### Link to Project: https://login-system-mvp.herokuapp.com/register

![login](https://user-images.githubusercontent.com/17926581/137521863-aef7aedf-9edc-4533-96af-ec0d5b48b1b4.gif)

## How It's Made:
Using Express for server backend and Passport to help manage the logged in state of users. 
Using bcryptjs to encrypt and hash all user passwords so that the application is completely secure. 


## Lessons Learned:
Understanding bcrpyt provides Salted hashing that could prevent rainbow table attacks by generating random bytes (the salt) and combining it with the password before hashing creates unique hashes across each user’s password.

Understanding PassportJS manages session user for us and gives us a lot of strategies to use when we want to integrate login/register options in our application.


bcrypt works in 2 steps — 
> A. Generate the salt first (if err throw err else give me the salt)
> 
> B. hash the password with the generated salt (passing a cb so if there’s error throw error else give me the hash).




## Things to improve:
This time I didn't use database to store data; instead, I used local storage to store user data for the sake of convenience.


