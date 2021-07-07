# ![GA Logo](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Auth Research Lab

---

Authentication is a complex and exciting topic that involves using many of the concepts we've already studied as well as several new ideas. 

An authentication system allows the registration / signup of new users and allows those users to sign in. It has to be able to identify each user and keep their information private and secure.

Being able to develop secure user login systems is in fact a whole career and life path in and of itself, but understanding the broad concepts of **Auth** is critically import for all developers. 

Describing auth flow and understanding key terms are very common **interview questions** for junior developers, so lets take some time to research and understand auth and the related concepts.

## Setup

Fork and clone this repository and answer the questions as you research directly in the README. You do not have to pull request and submit this lab, but you will want to have it on hand for reference in the future. 

## Auth Concepts Worksheet

#### Define the following

1. *Authentication*
   Serves to answer the question of who you are? Checks identity, login details to "authenticate."

2. *Authorization*
   What you can do or what you have access to.

3. Explain how *authentication* and *authorization* are related but distinct concepts.
   I would equate authentication as entering the front door of a house but authorization as telling you what rooms you can enter.

5. *Sessions vs Token based auth*
   A session requires state, and it's a server side creation of a session id stored as a cookie in the user's browswer, the user session is stored in the db or cache. 
   A token is stateless, and it's stored client side. When the user tries to access the server the server is responsible for verifying the token sent from the cookie.

6. *json web token (also know as a jwt)*
   Signed json object, contains validation of senders identity. Used for stateless auth, stored on client side. encoded NOT encrypted never put passwords in here. don't have to know whats inside, just how to decode it.

7. *Encoding, encryption and hashing* along with the uses for and differences between the three
   encoding changes the characters in a string based on a rule, encrypting uses an algorithm and key to make the data inscrutable, hashing creates a unique identifier and its not meant to store the data in a way thats not later retrievable, cant ever be unhashed. 

8. *oAuth* (pronounced oh-Auth)
   OAuth is an authentication protocol that allows you to approve one application interacting with another on your behalf without giving away your password. 

#### Explore and then describe the following npm packages:

1. [bcrypt](https://www.npmjs.com/package/bcrypt) - creates hash/salts passwords and stores them in a db
2. [jsonwebtoken](https://www.npmjs.com/package/jsonwebtoken)
3. [passport](https://www.npmjs.com/package/passport) - string of action it takes to authenticate
    * also describe what a *strategy* is in the context of this npm package

---

## Licensing
1. All content is licensed under a CC-BY-NC-SA 4.0 license.
2. All software code is licensed under GNU GPLv3. For commercial use or alternative licensing, please contact legal@ga.co.
