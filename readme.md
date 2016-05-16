![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png)

# Software Development Best Practices

### Why is this important?
<!-- framing the "why" in big-picture/real world examples -->
*This workshop is important because:*

Well-planned projects with flexible processes are more enjoyable to work on and turn out better. In the following workshop we will discuss how to plan appropriately and follow some best practices.

### What are the objectives?
<!-- specific/measurable goal for students to achieve -->
*After this workshop, developers will be able to:*

- Compare and contrast several development methodologies
- Define features as user stories
- Inform a UI with mockups
- Conduct a scrum

### Where should we be now?
<!-- call out the skills that are prerequisites -->
*Before this workshop, developers should already be able to:*

* Have projects in the planning phase

##Waterfall Methodology

![waterfall](https://i.imgur.com/yJMVO91.png)

Waterfall is a good example of a linear methodology in which the project's progress steady flows down from one team to another. It's "easy" manage due to the rigidity of the model.

###Consequences...

...

> What tends to happen to new projects in waterfall organizations?

## Agile Methodology

_Agile software development is a group of software development methods in which requirements and solutions evolve through collaboration between self-organizing, cross-functional teams. It promotes adaptive planning, evolutionary development, early delivery, continuous improvement, and encourages rapid and flexible response to change_- [Wikipedia](http://en.wikipedia.org/wiki/Agile_software_development)

The Agile Manifesto is a formal "proclamation" of key values for approaching software development put together in 2001. Let's discuss its core 12 principles:

* Our highest priority is to **satisfy the customer**
through early and **continuous delivery
of valuable software**.

* **Welcome changing requirements**, even late in 
development. Agile processes harness change for 
the customer's competitive advantage.

* **Deliver working software frequently**, from a 
couple of weeks to a couple of months, with a 
preference to the shorter timescale.

* Business people and developers must **work 
together** daily throughout the project.

* Build projects around **motivated individuals**. 
Give them the environment and support they need, 
and trust them to get the job done.

* The most efficient and effective method of 
conveying information to and within a development 
team is **face-to-face conversation**.

* **Working software** is the primary measure of progress.

* Agile processes promote **sustainable development**. 
The sponsors, developers, and users should be able 
to maintain a constant pace indefinitely.

* Continuous attention to technical excellence 
and **good design** enhances agility.

* **Simplicity**--the art of maximizing the amount 
of work not done--is essential.

* The best architectures, requirements, and designs 
emerge from **self-organizing teams**.

* At regular intervals, the team **reflects on how 
to become more effective**, then tunes and adjusts 
its behavior accordingly.


## Best practices

####Satisfy the Customer

* **User stories** define the features an application will provide in a simple and concise way.

* **Wireframes** define the user interface of the application.

####Deliver Working Software

* **Pair programming** is development technique in which two programmers work on a specific problem together.

* **Test-driven development** improves code design and quality.

###Work Together

* **Scrum meetings** are short meetings used to plan, review, and increase accountability and clarity across a team.

* **Retrospectives** a period for reflection at the end of each sprint.

## User Stories

###How do I know what the client wants?

When you meet with the client translate all the features that you discuss into **user stories** following the format:

**A user *(specified type optional)* can [GOAL], *so that [PURPOSE]***

For example:

- _A user can read reviews of a book (so that they are better informed when making a purchase)._
- _An admin can update the inventory of a book so that the buyers know what is available._

###How can I make an accurate time and budget quote on a project?

As a user story complexity increases linearly, its time to complete it will increase geometrically. As a result, when assigning weighing each user story's relative complexity assign it a fibonacci number that corresponds to the relative time it will require. This is called the **point system** and is a great way to budget time and money.

**[1, 2, 3, 5, 8, 13, 21]**

corresponds to:

**[easiest, easier, easy, moderate, hard, harder, hardest]**

*Note: If something is every bigger than 21 points, consider breaking it down into more user stories.*

Once all the user stories are assigned points, it is possible to start estimating how many points can be completed in a given period of time. A **sprint** is a period of predefined time, typically 1-2 weeks, during which teams aim to complete a set of user stories. The team initially estimates how many points is realistic to accomplish during the a sprint. Once the team completes a sprint, they can measure the rate of points completed in a given of time, or their **velocity**. Knowing the current and average velocities of the team, allows for more accurate projections into the future. 

A collection of user stories will contain an overall point score.

###What tools should I use to do this?

Head to [Trello](https://trello.com), make a new board, and create three lists: "To Do", "Doing", and "Done".

<figure>
  <img src="imgs/user-stories.png" alt="Kanban-style user stories">
  <br>
  <figcaption>Kanban-style user stories</figcaption>
</figure>

For each user story it is possible to break it down into sub tasks.

<figure>
  <img src="imgs/story-tasks.png" alt="user story tasks">
  <br>
  <figcaption>A user story's tasks</figcaption>
</figure>

> Challenge: Write an example user story either for tic-tack-toe or for an original game you are planning to build.

## Wireframes

Wireframes illustrate how the user **navigates** to and **interfaces** with **information** presented to them.

Having user stories will better inform wireframes, while having wireframes will help further refine the user stories. They are very complementary in this way.

Can the user intuitively **navigate** through the experience and **interface** with the **information** presented to them?

<figure>
  <img src="http://3.bp.blogspot.com/-8e_J8hkX_kM/TbSz0jywljI/AAAAAAAAAY4/Nei-hnfPGaI/s1600/Balsamiq+myTube+example.jpg" alt="example wireframe">
  <br>
  <figcaption>An example wireframe</figcaption>
</figure>

> Challenge: Wire frame the new page for [Tesla's Model 3](https://www.teslamotors.com/model3)

##Pair Programming

The practice of pair programming is cited to: **improve code quality** through an increase in communication, **facilitate team cohesion** through collective code ownership, **improve long-term velocity** through a reduction in errors made, in addition to other benefits! 

One programmer, the driver, writes code while the other, the navigator, reviews each line of code as it is typed in. The two programmers switch roles frequently.

![pair programming](http://i.imgur.com/cdiZYib.jpg)

Checkout [how Atlassian does it](https://www.youtube.com/watch?v=dYBjVTMUQY0)

##TDD

Test driven development will improve the design and quality of the code written. It follows the cycle:

![tdd flowchart](https://raw.githubusercontent.com/sf-wdi-26/modules/master/w08/d02/m3-testing-w-jasmine/img/tdd-flowchart.png)

*Note: pair programming and TDD can work well together in a [ping pong pattern](http://c2.com/cgi/wiki?PairProgrammingPingPongPattern).*

##Scrum

Similar to rugby, a **scrum** is when a team quickly groups up in an effort to "self-organize". It is recommended to keep the scrum as *short as possible*. Agree on a duration of about 5-15 minutes. Scrums are typically conducted at the very beginning of every day additionally as needed (i.e. afternoon and the end of the day). A standard format is to go around in a circle and for each person to answer the following questions:

* What user stories did you complete yesterday?
* What user stories are you working on today?
* Do you have any blocks?

*Note: a block is anything that has completely inhibited you from moving forward.*

> Conduct a scrum at your tables

##Retrospective

At the end of each sprint a team will conduct a **retrospective** in an effort to "become more effective". There are [numerous formats](http://retrospectivewiki.org/index.php?title=Retrospective_Plans) for which to conduct a retrospective; the six hats is a popular one.


###The Six Hats

**Blue Hat (5 minutes)**
Use the blue hat to discuss the objectives for the session and write the output on the whiteboard.

**White Hat (10 minutes)**
Participants raise and discuss anything from the last iteration which can be said to be a fact or information. Hunches and feelings and any discussion of reasons or other non information based output should be left for the appropriate hat.

**Yellow Hat (10 minutes)**
Participants can only talk about the good things that happened in the last iteration.

**Black Hat (10 minutes)**
Participants can only talk about the bad things that happened, any negative criticism they have or worst case scenarios they can think of.

**Green Hat (10 minutes)**
The discussion moves on to any ideas people have about solving problems or things that may add more value to the business or help in any way. Outside of the box helicopter view blue sky thinking is encouraged.

**Red Hat (5 Minutes)**
Give the participants a short period of time in which they can come up to the board and write down 2 emotive statements each. These could be the issues that have stood out for them the most or an idea for solving a problem. These statements should be instinctive which is why you will give them very little time to do this.

##Closing Thoughts

- How do user stories help manage a client/boss?
- In an organization that uses user stories and tdd how a client's feature request get translated into working code?
- Name two process a team can adhere to in order to improve the quality of the code produced.
- Name one way a team can better self-organize and improve to become more effective.

##Related Resources

* [Building an MVP](https://www.youtube.com/watch?v=1FoCbbbcYT8)
