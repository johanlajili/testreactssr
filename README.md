# React Isomorphic Boilerplate

## What is an isomorphic app?
An isomorphic app, also called universal app, is an app whose code is run both on the client and the server. It allows, on initial load, to send to the user a full page, already rendered, increasing load time by a **lot**. It also helps with SEO, allowing your JavaScript application to be properly referenced.

## Why should I use this boilerplate?
Honestly you shouldn't. Or any other boilerplate for SSR for that matter. I truly believe it's a subject too complex to be left to code generator that you don't understand. What you can do though is read through the code to find inspiration. I myself created this one by looking at multiple examples, frameworks and real applications to find my own flavour of SSR.

## What is the overall archictecture?
Without going into too much details, the application is cut into multiple **services**. 
* The ***universal-web-service*** is the main one, which serve the webpage to the user. When the user hits a route, it renders the application server side, including making HTTP request to other services, and sends it to the user. The client then makes call directly to other services when navigating. 
* The ***persistence*** service is responsible for dealing with storing and retrieving data to a database. In this particuliar use case I will use mongoDB, but any other DB would work.
* The **API-xxxx** services are all based on connecting another client 

[tbc]
