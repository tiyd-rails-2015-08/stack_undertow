# Stack Undertow

## Description

As students, you have spent a lot of time on StackOverflow.  However, now that you've been in the class long enough to have a few developer nightmares ("I just can't find the right answers!!!"), you've decided that it's time to build an improved version, and you've recruited students from another class to aid you in your quest.

## Objectives

After completing this assignment, you should...

* Be able to work from a set of existing user stories
* Be able to work in parallel with another team of developers
* Be able to write an API specification with a second team of developers
* Know how to integrate work across multiple codebases
* Gain experience resolving ambiguities in requirements and assumptions built into two different code bases

### Front End Objectives

After completing this assignment, you should...

* Be able to contribute to the design of a database and Domain Model
* Know how to write a User Interface (UI) for an API specification
* Gain experience writing reactive UIs with Angular JS

### Rails Objectives

After completing this assignment, you should...

* Be able to design a database and ReSTful API to support a range of features
* Know how to build an API to provide data to a reactive User Interface (UI)
* Gain experience writing high-throughput APIs with Rails

## Deliverables

* **A GitHub organization named...?** Create an organization in GitHub to represent your team for this project.  Give all team members full rights.
* **Two repositories named `api` and `gui`** The `api` repository will contain the Rails API code, and `gui` will contain the Angular JS interface.  Create both repositories under your GitHub organization's account.
* **A `README.md` for each repository** that describes each application and includes a link to the other project repo and the deployment URLs for each.
* **A Rails API deployed and running on Heroku.**
* **An Angular JS app served from Firebase Hosting**

### Before writing any code, produce the following:

* **A workflow diagram** describing the primary actions of the application in any format: pen(cil) and paper, whiteboard pictures, a formal drawing... whatever.
* **A data structure diagram** that should include:
  * A box for each table
  * Each field you'll need for each table
  * A data type for each field
  * A mark to indicate that it's a required field
  * Relationships between each pair of tables with a primary/foreign key link
* **A set of visual schematics** that should include:
  * Each page for the proposed application
  * Visual annotations denoting layout containers and important content areas
  * A mapping of content areas to API data

## Normal Mode

At its core, your application needs to allow users to ask questions, give answers, and vote.  You also need to provide anyone with the ability to search for questions and see answers.  Your application should allow the following actions:

* Site visitors can sign up for new accounts.
* Users can log in and log out.
* Users can post new questions.
* Users can answer questions.
* Users can upvote or downvote questions.
* Users can upvote or downvote answers.
* Site visitors (and logged in users) can view questions (and their answers and votes) without logging in.
  * When the site loads, top questions should be shown.
  * Search functionality should allow users to search for questions/answers, and have them appear sorted by quality.

## Hard Mode

If you complete the basics, you should begin awarding points for certain actions on the site, and keep track of how many points each user has acquired.  Your application should allow the following actions:

* Users can receive points for posting questions, posting answers, or receiving upvotes.
* Users can lose points for receiving downvotes.
* Question poster can set a bounty on a question.
* Question poster can award a bounty for an answer to a question with a bounty on it.
* Site visitors can see a leaderboard of users.

## Nightmare Mode

Once you have a point system in place, you can take more advanced actions based on these points.  Your application should allow the following actions:

* Users should receive badges for accomplishing certain things in the application.  Stack Overflow's system can be found [here](http://stackoverflow.com/help/badges).  Choose at least five of these badges and implement them in your system.
* Users should only be able to perform certain tasks once they have acquired a certain number of points.  Stack Overflow calls these "privileges," and their system can be found [here](http://stackoverflow.com/help/privileges).  Implement the following privileges:
  * A certain number of points (more than zero, you choose the threshold) needed to create posts
  * A higher number of points (you choose the threshold) needed to upvote
  * A higher number of points (you choose the threshold) needed to set a bounty
  * A higher number of points (you choose the threshold) points needed to downvote
