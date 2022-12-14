# OAuth

OAuth is a framework to provide applications better and more secure access or we can say we will be "outsourcing" the authentication process to a centralized login page in the same way that Gmail, YouTube, and any other Google property redirects to accounts.google.com whenever a user signs in, It allows you to sign up for an application using one of your profiles (Google, Facebook, LinkedIn etc.) without sharing your profile password. Instead it authorize tokens to interact between your profile and application. One of the example is like a one of the Dating site use your Facebook/Google profile for signup.
Following image depicts the flow of OAuth access management:

 ![image](https://user-images.githubusercontent.com/39763460/207592472-62eca6d4-88f2-4649-8171-5a5cfe78ff72.png)

In above image point 2,3,4,5 are the main steps that shows how OAuth works, this is where validation happens for authorization and providing secure tokens to application on behalf of you socials Ids.
When app needs to fetch user data from API:
1.	If the user is not already authenticated, SDK redirects the user to Auth0 Authorization Server.
2.	The user authenticates with Auth0 using one of your configured login options (e.g., username/password, social identity provider, SAML).
3.	App requests an ID Token and Access Token.
4.	Auth0 responds with the requested tokens.
5.	The Access Token can be used to call the API and retrieve requested data.


# Stripe

Stripe is a cloud-based service that enables businesses and individuals to receive payments over the internet and offers both client-side libraries (JavaScript and native mobile) and server-side libraries (Java, Ruby, Node.js, etc.).
Stripe provides a layer of abstraction that reduces the complexity of receiving payments. As a result, we don't need to deal with credit card details directly – instead, we deal with a token symbolizing an authorization to charge.
In this tutorial, we will create a sample Spring Boot project that allows users to input a credit card and later will charge the card for a certain amount using the Stripe API for Java.

![image](https://user-images.githubusercontent.com/39763460/207593744-fa6ab031-888b-4e59-9222-d613a7d37d77.png)

