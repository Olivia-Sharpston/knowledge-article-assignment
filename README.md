# What are Agile handoffs? What is their importance?
To break down what **Agile handoffs** are, let us start with breaking up the actual word. **Agile** refers to being able to work in smaller pieces, which allows better feedback when working on a project. **Handoff** refers to being able to give or transfer work or information to someone or something else, even it if is yourself. Together, **Agile handoff** is essentially passing on the pieces of work for the future or for someone or something else; therefore, progress is not lost or completely stuck. 

These are two of the main types of handoffs: self-handoffs and team handoffs. **Self-handoffs** are those where one leaves, or hands-off, the work and progress to their future self. **Team handoffs** would be handing it off to another work mate. However, self-handoffs are just as important as team handoffs. If working alone, it is very important to be able to pick back up where you left off without being lost or confused, such as if the weekend or some days have passed since it was last worked on. Therefore, it is important to be able to realize what is going on or what was last done in a project that is being done solo. Being able to do this adds to being able to [understanding the code](https://amymhaddad.com/why-reading-code-matters) as well, which is very important when working with code. 

---

### Benefits of Using Handoffs in Code:
* Helps Functionality
* Helps Reduce Debug Time
* Team Friendly Method
* Allows Reuseable Code to be Seen Easier
* Reduces Breaking Code, Especially When New Code is Added

If you would like to look more into team handoffs, this is a blog that goes more indepth in team handoffs: [Team Handoffs Blog](https://www.mountaingoatsoftware.com/blog/agile-collaboration-what-it-is-how-it-feels-and-why-it-matters)

---

# When setting up my Node app.
When setting up my Node app, I had to work in pieces. This project had occured over several days and work sessions. Furthermore, this project lead to many back-and-forths through different tabs, files, and saves. While working on my Node app, I would leave comments throughout the project. These comments would appear in the middle of some code chunks and before chunks of code. The comments before the code would more than likely be there to explain what was happening below the comment. This helps me and anyone else looking, working, or reading through the code to have a better understanding of what was happening in the code. The comments that would be in the middle of code chunks would be there if I had to stop working and/or the code has several pieces in a chunk of code. 

Putting in the comments in my Node app would be a way of self-handoffs. These comments allow me to come back and see what was done the last time work had been done in the app. I have done this for several years among several platforms, such as Python, Eclipse, C++, etc. This method has worked for me, if not every time, almost every time. This is a method that I definitely recommend when working on something over a course of time, especially when by yourself.

---

### Examples of Self Handoff in Code
This shows how self handoffs were used in the Node app within a code block. This allows for me, or anyone, to be able to better understand what is going on when looking through my Node app.
``` js
async function run() {
  try {
    // Connect the client to the server	(optional starting in v4.7)
    await client.connect();
    // Send a ping to confirm a successful connection
    await client.db("admin").command({ ping: 1 });
    console.log("Pinged your deployment. You successfully connected to MongoDB!");
  } finally {
    // Ensures that the client will close when you finish/error
    await client.close();
  }
}
```

---

Below is a snippet of code from my app.mjs file from my Node app. In this first line of code, you can see that is starts with two backslashes. This is how a comment is made on this file. Different platforms and file extensions have different syntax for starting a comment. 
``` js
// Create a MongoClient with a MongoClientOptions object to set the Stable API version
const client = new MongoClient(uri, {
  serverApi: {
    version: ServerApiVersion.v1,
    strict: true,
    deprecationErrors: true,
  }
});
```

---

Below is an example of a comment from an HTML file. As you can see, the comment looks different here. These comments begin with "<!--" and end with " -- >". 
``` js
<!-- <hr>
<form id="postForm" method="get" action="/api/body">
  <label>POST (body): </label>
  <input id="postFormName" name="name" placeholder="Enter name">
  <input id="postFormZipCode" name="zip" type="number" placeholder="Enter zipcode">
  <button type="submit">Submit POST</button>
</form>
<div id="postFormResult"></div> -->
```

---

If you would like to start adding comments into your code, here is a citation that can help you get started with formatting comments to help them be more legible: [Code and Comment Styles](https://mitcommlab.mit.edu/broad/commkit/coding-and-comment-style/)
