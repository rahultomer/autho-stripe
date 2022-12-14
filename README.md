<<<<<<< HEAD
# Spring Boot 2 Login - MVC

This sample demonstrates:

- Adding authentication with Auth0 to a Spring Boot 2 MVC application
- Accessing profile information of the authenticated user
- Only allowing authenticated users to access certain resources

## Configuration

### Auth0 Dashboard
1. On the [Auth0 Dashboard](https://manage.auth0.com/#/clients) create a new Application of type **Regular Web Application**.
1. On the **Settings** tab of your application, add the URL `http://localhost:3000/login/oauth2/code/auth0` to the **Allowed Callback URLs** field.
1. On the **Settings** tab of your application, add the URL `http://localhost:3000/` to the **Allowed Logout URLs** field.
1. Save the changes to your application settings. Don't close this page; you'll need some of the settings when configuring the application below.

### Application configuration

Copy `src/main/resources/application.yml.example` to `src/main/resources/application.yml`:

```bash
cp src/main/resources/application.yml.example src/main/resources/application.yml
```

Set the application values in the `src/main/resources/application.yml` file to the values of your Auth0 application.

```yaml
client-id: {YOUR-CLIENT-ID}
client-secret: {YOUR-CLIENT-SECRET}
issuer-uri: https://{YOUR-DOMAIN}/
```

### Running the sample

Open a terminal, go to the project root directory and run the following command:

Linux or MacOS:

```bash
./gradlew bootRun
```

Windows:

```bash
gradlew.bat bootRun 
```

The application will be accessible at http://localhost:3000.

### Running the sample with docker

In order to run the example with [Docker](https://docs.docker.com/install/) you need to have `docker` installed.

You also need to set the client values as explained [previously](#application-configuration).

Execute the command to run Docker for your environment:

Linux or MacOS:

```bash
sh exec.sh
```

Windows:

```bash
.\exec.ps1
```

The application will be accessible at http://localhost:3000.

## Issue Reporting

If you have found a bug or if you have a feature request, please report them at this repository issues section. Please do not report security vulnerabilities on the public GitHub issue tracker. The [Responsible Disclosure Program](https://auth0.com/whitehat) details the procedure for disclosing security issues.

## What is Auth0?

Auth0 helps you to:

* Add authentication with [multiple authentication sources](https://docs.auth0.com/identityproviders), either social like **Google, Facebook, Microsoft Account, LinkedIn, GitHub, Twitter, Box, Salesforce, amont others**, or enterprise identity systems like **Windows Azure AD, Google Apps, Active Directory, ADFS or any SAML Identity Provider**.
* Add authentication through more traditional **[username/password databases](https://docs.auth0.com/mysql-connection-tutorial)**.
* Add support for **[linking different user accounts](https://docs.auth0.com/link-accounts)** with the same user.
* Support for generating signed [Json Web Tokens](https://docs.auth0.com/jwt) to call your APIs and **flow the user identity** securely.
* Analytics of how, when and where users are logging in.
* Pull data from other sources and add it to the user profile, through [JavaScript rules](https://docs.auth0.com/rules).

## Create a free account in Auth0

1. Go to [Auth0](https://auth0.com) and click Sign Up.
2. Use Google, GitHub or Microsoft Account to login.

## Issue Reporting

If you have found a bug or if you have a feature request, please report them at this repository issues section. Please do not report security vulnerabilities on the public GitHub issue tracker. The [Responsible Disclosure Program](https://auth0.com/whitehat) details the procedure for disclosing security issues.

## Author

[Auth0](https://auth0.com)

## License

This project is licensed under the MIT license. See the [LICENSE](../LICENSE) file for more info.
=======
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

>>>>>>> 31ebdff2abba699c57eb63a730759866ecbc7196
