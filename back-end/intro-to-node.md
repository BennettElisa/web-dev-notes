## Node Read Evaluation Print Loops (REPL)

- Allows you to excute code in bite size chuncks
- When we installed Node we also installed Node REPL

  - REPL is accessable in the terminal by typing "node"
  - Once you see the little angle bracket you know your inside the REPL ">"

  ![REPL](images/REPL-bracket.png)

Now, we'll look at some **native node modulos** which simply means **packages of code** that has be **bundled** in to Node.js to make our lives easier.

When we install Node.js it already comes bundled with many built in modulos. These modulos are **libraries of code** that the design team wrote to help us with day to day things that we want to do.

We can use Node.js to get direct access directly to the files on the local computer.

To use different modulos in our code we have to use the **require** keyword.

For example, if we want to use a Node.js modulo that gives us access to our file system then within our index.js file we would write the following code :

![A Node Modulo](images/copyFiles.png)

This allows us to copy files in the same folder that we are currently inside of.

Next we'll look at **external modulos**

## External Modulos - NPM Package Manager

**Node Package Manager**

- bites of reusable code that someone else wrote
- using npm you can incorporate the packages into your our code
- npm COMES WITH NODE.JS

We can now use **npm init** to create a **package.json** which is our own package. When we run **npm init** in our Command Line it will ask us a series of questions about our package. Then, you will see the new **package.json** file that holds the information we entered in an object literal.

![npm-init](images/npm-init-created-this.png)

You just created your first node.js package! 📦

![package-jason](images/package-jason-icon.png)

If you were to click on this new file in your project directory you will see an object literal. This object literal give you a description of all of your npm packages aka it tells you about all the packages you have installed inside of your project.

Once we install external package it will also show up in our **package.json** file.

## Installing an external package

1. Visit [npm](https://www.npmjs.com/package/superheroes)
2. Search for a package
3. Follow install instructions
4. Follow usage instructions

![VS Code Example](images/external_modulos_npm.png)

# Express (a Node.js Framework)

Express is a Node.js framework - escentially a bunch of code that someone else wrote that helps to structure and organize your code.

** Great Analogy**

Node.js is the screw driver
Express is the power drill

The screw driver can do a lot of things but at some point your DIY project will require more than a screw driver and this is when you pull our your power drill 🧰

Express was built to help write less repetivtive code when building web applications and is made for web developers. It can save you 5 to 10 times the amount of code that you'd need to write.

 <!-- Include pictures from command line in setting up package for server -->

This is the process that you will go through **each time** you create a **new web development project**.

After you've created your package you will now install express with the following command on the command line '''npm install express'''

You will now see the **node_modulos** folder in your directory and your **package.json** file will show **Express** as a dependency.

Now that we've installed **Express** the next step is to **REQUIRE** it in our server.js file.

[Hello World Example](https://expressjs.com/en/starter/hello-world.html)

# Set up and START Server

This sends an HTTP request on the port that we've selected.
If we want to see when our port is set up and **when our server is running** we can add a **callback** to the **listen method.**

<!-- insert code  and cannot get from localhost:3000 -->

This means that when our browser is trying to get in touch with our server on the port 3000 it's not able to get anything back. So the next step will be to write code so that our server responds when our browser is making a request to our server we have to send information to the browser to display.

# Browser makes GET request

Currently our browser is staying "Hey! I got in touch with your server at this location 3000 but I couldn't get anything back because your server didn't pick up."

localhost:3000 is the same thing as "root" of any page meaning the "home page" of any web domain i.e www.google.com

Another example --> when we type in www.google.com OUR browsers send a request to Google's servers to get some data for this location. And google servers - when it see the request - will send our browser a response. This is where the magic happens --> that response includes the HTML, CSS and JavaScript to render the site.
