### Conceptual Exercise

Answer the following questions below:

- What is the purpose of the React Router?

 with react-router, you can get "client-side routing". Moving around site doesnt require server load, URL bar/bookmarks and back-forward button will work.

- What is a single page application?

 sites that exclusively use client-side routing are single-page applications.

- What are some differences between client side and server side routing?


 Sever-side routing is the traditional pattern, server decides what html return based on URL requested.
Client-side routing handles mapping between URL bar and page user sees via browser rather than server.

- What are two ways of handling redirects with React Router? When would you use each?

one is using <Redirct> component, another one is calling .push method on the history object.

- What are two different ways to handle page-not-found user experiences using React Router? 
 first is to add <Route><NotFound /> </Route>
 another is to redirect to some page else.


- How do you grab URL parameters from within a component using React Router?
 we indicate a URL parameter with the colon:. Then useParams() will return an object with keys.

- What is context in React? When would you use it?
  
  Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

- Describe some differences between class-based components and function
  components in React.
  
  Functional Components:
 1. A functional component is just a plain JavaScript function that accepts props as an argument and returns a React element.
 2. There is no render method used in functional components.
 3. Also known as Stateless components as they simply accept data and display them in some form, that they are mainly responsible for rendering UI.
 4. React lifecycle methods (for example, componentDidMount) cannot be used in functional components.
   
   Class Components:
  
  1.A class component requires you to extend from React. Component and create a render function which returns a React element.
  2.It must have the render() method returning HTML
  3.Also known as Stateful components because they implement logic and state.
  4.React lifecycle methods can be used inside class components (for example, componentDidMount).
  
  
- What are some of the problems that hooks were designed to solve?

 Function and class components appeared in React at the same time. However, function components originally could not contain state or make use of lifecycle methods.Even with this limitation, function became popular when they could be used.
Using certain tools, such as redux, also made it easier to build applications without needing many class components.

 With the advent of hooks, we can now use function components all the time!