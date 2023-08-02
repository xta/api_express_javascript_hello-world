# Express.js/JavaScript: API Basic Access Control Code Sample

This JavaScript code sample demonstrates **how to implement authorization** in Express.js API servers using Auth0.

This code sample is part of the ["Auth0 Developer Hub"](https://auth0.com/developers/hub), a place where you can explore the authentication and authorization features of the Auth0 Identity Platform.

Visit the ["Express.js/JavaScript Code Sample: Authorization For Basic APIs"](https://auth0.com/developers/hub/code-samples/api/express-javascript/basic-authorization) page for instructions on how to configure and run this code sample and how to integrate it with a Single-Page Application (SPA) of your choice.

[![Express.js/JavaScript Code Sample: Authorization For Basic APIs](https://cdn.auth0.com/blog/hub/code-samples/api/express-javascript/basic-authorization.png)](https://auth0.com/developers/hub/code-samples/api/express-javascript/basic-authorization)

## Why Use Auth0?

Auth0 is a flexible drop-in solution to add authentication and authorization services to your applications. Your team and organization can avoid the cost, time, and risk that come with building your own solution to authenticate and authorize users. We offer tons of guidance and SDKs for you to get started and [integrate Auth0 into your stack easily](https://auth0.com/developers/hub/code-samples/full-stack).

## Setup

    touch .env

    ##Enter (with your own values) in .env

    PORT=6060
    CLIENT_ORIGIN_URL=http://localhost:4040
    AUTH0_AUDIENCE=https://hello-world.example.com
    AUTH0_DOMAIN=YOUR_DOMAIN.us.auth0.com

## Usage

    npm run dev


    curl --request GET \
      --url http:/localhost:6060/api/messages/protected \
      --header 'authorization: Bearer TOKEN_GOES_HERE'

      //=>
        {
          "text": "This is a protected message."
        }


