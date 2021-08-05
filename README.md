# typescript-code-scanner
A library that allows extracting specified code usage in a TypeScript program.

## Example
Let's say you have a UI written in React created with create-react-app. You also have a backend with an exposed API that's using Swagger from which you can grab the API json (e.g. https://petstore.swagger.io/v2/swagger.json).
So you've generated TypeScript types and services from that API json using openapi-generator for example. You started using those services in your React app.
Then, somebody asks you - what API endpoints are you using? Ok, give me some time ... 15-30 mins later, depending on the project's size, you send that person a list of API endpoints that you have to reverse engineer from the generated services' usage.

Comes ... typescript-code-scanner!

With typescript-code-scanner you're able to write a simple config and some processing functions for your project and then just run it from cmd line - voilà! You have the list of endpoints someone asks of you. Next time you get this request, you'll reply withing 1-2 mins, even if your UI changed drastically with regards to the API and its usage.

## Resources
- https://learning-notes.mistermicheels.com/javascript/typescript/compiler-api/
- https://github.com/Microsoft/TypeScript/wiki/Using-the-Compiler-API
- https://github.com/OpenAPITools/openapi-generator
- https://dev.to/unhurried/typescript-rest-api-client-4in3
- https://tech.smarthr.jp/entry/2020/08/25/135631
