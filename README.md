# Stand-Ups
This is tracking sheet for me to keep track of my progress / Learning / Daily task
# 11/15/2018
Today my main focus was continue learning react. The concept of building independent components is a really powerful feature of react. Each component has different states and we can use those states to build rich powerful ui friendly application. 
# 11/17/2018
Today learned more about the presentation layer of web components. React has two library React and ReactDom. React library has function used for creating components and for making componets talk nicely together. ReactDom takes those components and renders them to the document object modal. React heavily centered on presenting content to users and reacting to user interaction with components. since the later version of JS are poorly supported with most browsers. We have to use a command line tool called babel to compile later version of Javascript into a suported of Js. React uses Es2016 so we have to make sure we includ our babel dependencies in order to compile React code into a friendly version of JS supported by most browsers. 
# 11/19/2018
More In depth learning about JSX. basicaly a sepcial dialect of Js. It renders content for the user to see. A componrt is a function or class that renders html content. There are differences between JSX and Html. Some of those differences are using className to reference a class attribute. We can interpulate js using {} syntax. We can render objects to show in the UI. that will cause errors. If we want to show a text from a object we have to reference a property in that object. More knowledge on whar Component nesting, resuability, and configuration means. 
# 11/20/18
Learned about React prop system. It allows us to customize and configure components in our application. It gives us the ability to reuse componetns with different data. Configure the component depending on the ui requirement. Also it allows us to pass data from the parent to the child components. 
# 11/24/18
Within components We can update the state of a component depending on revelant data associated with the components. The dofference between functional components vs class components. Is when we can to just render JSX to show some content we use functional component. While class component is best when we want to build some logic or handle component state. The only time we want to assign value to a component direcelty is through the constructor. if we want to update a state for a given component we use the setState() method. 
# 11/26/18
Class componets are easier to organize code and gives the ability to handle state. Class componets also allows to better use component 
lifecyele. Functional components are best to be used to render content to the user. callback functions are function that will be called at some point in time. If we are passing a callback function inside a event handler we do not add parenthesis because it will called every time the component is rendered. 

# 11/27/18
Call back functions get called at some point in time in the future.
We never put parenthesis to functions we passes in event handlers because they
are callback functions. Everytime we render the componenet the function will be called. 

controlled vs Uncontrolled
Again any time we call setState the component will re render itself because 
your updating the state. 

Controlled- As developers we want to centeralize information inside our React
components than in html. We dont want to store data in the DOM. 
We want React driving and storing our data in components. 
this is always going to be equal to the instance of a class. 
When looking at the value of this inside a function. You look where the function being called. 

# 12/1/18
Arrow functions do NOT define their own this, they go to enclosing scope and look for it just as they would with any variable you try to use in their scope.
When we pass values in props and callback function that we author we can call them anything we want. 
REACTS Job is showing content to the user and handling user interaction. Not to ajax requests.
lecial scope is what variables I have access to. Where variables are being defined
Context is the value of this.
Axios 3rd party package 
fetch function built into modern browsers

# 12/3/18
Learned how to pass in data from axios request using props form parent to child. 
Pass in a list of data and render them dynamically on the browser.
how to use the ref system to access the dom from a rendered component. 
using the .map function to return a new list of array without using a forloop. 
css grid system. 
destructing objects using es6 feature for better code readbility. 

# 12/5/18
Solidfying more on parent and child components. To access component elements within the dom. 
Use the ref system for DOM node element. More on http request using axios. Implementing a Youtube search app.


# 12/8/18
Implemented a video search application. This app used youtube api to respond to a user request for a specific video. Learned about how to pass information from children back to parent using callback function. This alows for communication between child and parent. 

# 12/11/2018
Node-
      JavaScript runtime used to execute code outside of the browser
      JS was originally always excuted on the browser. To make website interactivity. 
      Node is simply used to excute code outside the web browser.
	
express-
	Library that runs in the Node runtime. Has helpers to make dealing with Http traffic. 
	express a collection of function and helpers to make http accepts of Node js easier to work with.
	express looks at request and decided what chunk of code will handle a respond to request.
	we write a collection of route handlers responds to request. Different route hanlders respond to incoming
	request. Generate a resposnse to the incoming request. 
	
Dynamic port binding-
	on server side we use commonJS modules. System implemented in node js to share files. 
	enviromnet variables are variables that are set in the underlying runtime node is running on. 
	Heroku tells which port our app will use. proces.env.PORT.
	
PassportJS-
	The core base passport library or module is a set of very general functions and objects. 
	That make authentication work nicely inside express. Generic logic that can handle the idea of authentication
	with express. Passport a general helper library for handling auth express apps
	passports strategy is for authenticating with one very specific method
	(email/password, google and facebook)
	Different strategy offer different methods of signing logic.
	strategy is a module that helps you authenticate with one specific provider. 
	
# 12/15/2018
 -The Theory of Authentication
	Http is stateless.
	We communicate between client and web server by http request.
	Known as REST(REPRESENTATIONAL STATE TRANSFER)
	AJAX Request are still Http request and stateless.
	This means that any two given request that make Http request.
	Have no way of identifying or share information between two seperate request.
	By default information between request are not shared.
	So we cant identitfy who is making any request between any given number of request. 
	
	We cannot rely upon HTTp to authenticate users. This is due to Http being stateless. It does not
	keep track of information being sent to the webserver. The solution is the server providing some token 
	that it can trust upon authenticating users. 
	
	 -Cookie based authentication
	 the entire idea behind cookie authentication. Is that the web server 
	 puts some identifying piece of information into the users cookie that is going
	 to be cached in the browser memory. This piece of information will be set in some 
	 property within the request header that will be used to identify users during any request 
	 sent to our web server. The web server will use this cookie to authenticate our users .
	 
	 -OAuth Flow
	 OAuth main purpose is to give us a unique identitfying token that we trust.
	 
	 -MongoDb
	 stores its information in collection. 
	 within collection we have many records
	 every record is a plan JS Objects: Key value pairs 
	 Defining characteristis of MongoDb is the fact that is schema less. 
	 Meaning every record can have its own distinct set of properties. Unlike
	 relational database system tables which must have a schema before any data is inserted in a table.
	 
	 -MongooseDb
	 A model class created with Mongoose represnets an entire MongoDb collection. 
	 model class is used to access a single collection sitting inside MongoDb Model class. 
	 Mongoose would classified as an ORM that helps maps models to collection. 
	 Model instances represnets a record in a collection. 
	 
	
# 12/22/2018
middleware are small function that can be used to modify incoming request to our app before they are sent of to route handlers.
middleware do preprocessing incoming request before they are sent off to different route handlers

Architecture 
We have our React app front end side
and express server back end side
-React front side bundles our different js files into one front app to display
-express back end side handles business logic we create new users and authentication.

# 12/31/2018
Redux
	-State management library
	-makes creating complex applications easier
	-Stablize complexity as an application begins to grow. 
	
	
Redux Cycle
	- Action creator -> Action -> dispatch -> reducers -> state
	- Action creator - its purpose is to create a action. its a function that returns
	 a plain JS Object. 
	 Action- its purpose is to describe some change in the data we want to make a change
	 Dispatcher - its purpose take an action makes a copies of the action and pass it to different
	 reducers in the application.
	 Reducers- its responsible for taking existing data and a action updating that data based on the logic
	 state- centarilized location for storing data processed by the reducers.
	-every time we want to change the state of our app we call action creator
	 a redux dispatch runs the whole redux cycle.	 

	 
