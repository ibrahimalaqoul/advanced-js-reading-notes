# class 06 Reading :
## securing password :

**Here i'm talking about secring passwords with Bcrypt Hashing functions.**


The general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible. Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.

#### PROBLEMS WITH CRYPTOGRAPHIC HASH ALGORITHM :
* Brute Force attack.
* Hash Collision attack.

#### **BCrypt, IT's SLOW AND STRONG** 
#### To overcome such issues, we need algorithms which can make the brute force attacks slower and minimize the impact. Such algorithms are PBKDF2 and BCrypt, both of these algorithms use a technique called Key Stretching.

This hashing algorithm is implemented in a number programming languages like Javascript , PHP, Java, Ruby, C#, C etc. 


## Basic Authentication :
In HTTP transaction, basic access authentication is a method for an HTTP client to provide a user name and password when making a request. 

The BA mechanism does not provide confidentiality protection for the transmitted credentials. They are merely encoded with Base64 in transit and not encrypted or hashed in any way. Therefore, basic authentication is typically used in conjunction with HTTPS to provide confidentiality.

## Authentication  :
Authentication is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

### Session Management
 is a process by which a server maintains the state of an entity interacting with it.

## Authentication Responses

* The user ID or password was incorrect.
* The account does not exist.
* The account is locked or disabled.

