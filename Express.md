# Express.js {FrameWork}

## User Interface Frameworks
* Bootstrap
    * Very well known and built by Twitter
    * Easy to learn and looks professional
    * Can be easy to spot "Bootstrap Sites"
    * Can be difficult to customize components
* Materialize
    * Clean looking
    * A bit more "fun" than Bootstrap
    * Lots of styling and color options
    * Follows Google's Material style guide
* Foundation
    * Lots of examples
    * Professional looking
* Semantic UI
    * Lots built-in
    * Built-in themes so it's customizable
* Grommet
    * Has a huge focus on accessibility
    * Looks really clean
    * Not as used as some of the others
    * Made for React JS (another framework we will look at later)


## Frontend Frameworks
* Frontend frameworks are, in most cases, written in JavaScript and are for organizing the functionality, interactivity of your website. Some of these include:

* Vue
    * Easy to learn
    * Very fast
    * All tools associated with it are packaged well
    * Takes parts from Angular and React and optimizes them
    * less widely adopted than some others
    * Flexible -- you can use it in multiple ways
* AngularJS
    * Built by Google
    * Well supported
    * Huge number of features
    * Improves application scalability
    * Difficult to debug
    * Large learning curve
* Angular 2+
    * Built by Google
    * Well supported
    * Encourages reusability
    * Improves application scalability
    * Large learning curve
* React
    * Built by Facebook
    * Bundles frontend code into components
    * Organizes code and data to make code more reusable
    * Large learning curve
* Ember
    * Gives a large amount of functionality out of the box
    * Opinionated (you have to use its formatting)
    * Steep learning curve

## Backend Frameworks
* Backend frameworks are a lot more varied. They are written in a variety of programming languages and have a wide variety of features. Below, like the above list, is a very incomplete list of some of the frameworks out there for writing application backends.

* Spring MVC
    * Java (more difficult language to learn)
    * Very fast
    * Less opinionated
* Django
    * Python (easier language to learn)
    * Happy medium between being very opinionated and less structured
    * Gives you a lot of functionality out of the box (like user authentication, database connections, and view rendering)
    * Can be difficult to integrate a fancy front-end.
    * Python's data handling is amazing
* Flask
    * Python (easier language to learn)
    * Less opinionated and more customizable than Django
    * Gives you less out of the box (you have to build more)
* Ruby on Rails
    * Ruby (easier language to learn)
    * Very opinionated
    * Has great tools like scaffolding so you can build things fast
    * Gives you a lot of functionality out of the box (like user authentication, database connections, and view rendering)
    * The asset pipeline helps with front-end development
    * Ruby takes longer to run programs than some other programming languages
* Meteor
    * JavaScript (easier language to learn)
    * Gives you a lot of functionality out of the box (like user authentication, database connections, and view rendering)
    * Integrates very well with modern front-ends
* Express
    * JavaScript (easier language to learn)
    * Very customizable
    * Very lightweight
    * Less built-in features
    * Node is very fast


## Routes

* Routes essentially just match a request’s HTTP verb (e.g. GET or POST) and URL path to the appropriate set of middleware functions - the controllers

```jsx

app.get("/", (req, res) => res.send("Hello, world!"));

```
* app.get "/" ... tells us that this route will match any GET requests that go through the app router (which is our whole server!) to the / path. If instead we had the following:

 ```jsx
 app.post("/messages", (req, res) => res.send("This is where you can see any messages."));

```
* That would tell us the route matches any POST requests to the /messages path of our app. If you sent a GET request to the /messages path, it would not match this route
* Each HTTP verb has its own Express route method, and you can also use app.all() to make a route match all verbs

## Paths

### Route parameters

```jsx
app.get("/:username/messages", (req, res) => {
  console.log(req.params);
  res.end();
});
```
* So : is used when that part of the URL can change. If the path is always fixed, then no need for :
* here we can get diff user namess..

```jsx
app.get("/:username/messages/:messageId", (req, res) => {
  console.log(req.params);
  res.end();
});
```
* here we can get digg username and message ID

    ```
    Example :

      Imagine you are building a social media site. You can't hardcode a separate URL path for every single user on Earth (e.g., /odin/messages, /thor/messages, etc.).

    Instead, you use Route Parameters to create a placeholder or a wildcard in your URL structure.

    How you write it in code: You use a colon (:) followed by a variable name.

    "/:username/messages"

    How Express reads it: When a user visits a URL, Express takes whatever is written in place of :username and stores it inside an object called req.params
    ```

### Query parameters

* A **?** denotes the **start** of the query parameters and each query **separated** by an **&**

* While route parameters define the structure of the path, Query Parameters are used to sort, filter, or pass extra optional arguments to that path. They always appear at the very end of a URL

```
Example:

If a user goes to /odin/messages?sort=date&direction=ascending:

Express still routes them to the /:username/messages path.

But it extracts the extra details and creates this object:
req.query = { sort: "date", direction: "ascending" }

Note: If someone repeats a key (like ?sort=date&sort=likes), Express is smart enough to group them into an array: { sort: ["date", "likes"] }
```

### The Real-World YouTube Example
* The text uses YouTube to show you how you already use this every day:

    * When you watch a video, the URL looks like this: https://www.youtube.com/watch?v=xm3YgoEiEDc&t=424s

        Behind the scenes, YouTube’s servers receive this request. Because of the ?, they parse the query parameters into an object like this:

       ![alt text](image-1.png)

## Diff
* **Route Parameters** (req.params): Built into the URL path itself (/users/:id). Used to determine what resource you are looking at.

* **Query Parameters** (req.query): Appended to the end of the URL (?search=shoes&size=10). Used to filter, sort, or modify how that resource is displayed.
