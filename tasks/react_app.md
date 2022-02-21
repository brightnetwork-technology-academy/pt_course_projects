# Building a Web App With React

In week 2 we built an API which we could use to record details of BNTA's consultants and clients. By keeping the front-end separate we have ensured that anyone could build an app and connect to it so long as their requests follow the correct pattern. In this task we'll use React to do just that!

## Task

Use React to build a front-end for the API you created in week 2. The app should be able to make requests to every route specified in the week 2 task and display the information received. As a reminder the routes allow the user to:

- add a client
- add a consultant
- view all clients
- view all consulatants
- view individual clients
- view individual consultants
- update a consultant with new location and/or cient details
- view all consultants working at a given client
- view the client a given consultant is working for

How this information is displayed on the front-end is up to you. Information from multiple routes can be handled within a single component, eg. displaying the details of a specific client could include a list of the consultants working there.

Try to keep your code DRY by minimising the number of components you need.

Your backend won't currently accept connections from your React app. Add [CORS configuration](cors.md) to allow the appropriate requests from `localhost:3000`.

## Possible Extensions

- Use React Router to improve navigation in your app
- Add CSS to your app to improve its appearance:
	- Consider making your app mobile-friendly by adding media queries
	- Alternatively, research some CSS libraries (eg. [Bootstrap](https://react-bootstrap.github.io/), [UIkit](https://getuikit.com/docs/introduction)) and incorproate one of them. Make sure you use the React version if one is available!