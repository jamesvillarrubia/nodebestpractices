# Consider all the consequences when choosing the main framework

<br/><br/>

### Recommended frameworks: Pros and cons

Unlike other choices, choosing the core framework determines strategic factors like the development style and how likely the team is to hit a wall. We believe that framework popularity is a supreme consideration and put our focus on the top 4 most popular frameworks in terms of downloads and GitHub stars. The text below outlines the pros and cons of each framework and how to match a framework to the right application type

**express.js**

Pros: Unmatched popularity; gigantic eco-system of extensions and middleware; simple to learn and use; familiar to almost every Node.js developer; tons of community articles and videos are based on express

Cons: Covers a small subset of a typical application needs - merely a web server that invokes the app function per URL. Choosing express means leaving a handful of app concerns uncovered; outdated mechanics - no native support for async-await; barely maintained and updated; Slower than others

**Nest.js**

Pros: More batteries than any other option - covers many application concern including message queues, scheduled jobs and more; OOP-style is an advantage for teams who appreciate this design style; awesome docs; well-maintained; high popularity with a vibrant community

Cons: High-level abstractions that cloud built-in Node.js conventions; The inclusion of many features, heavy usage of TypeScript and reference to sophisticated patterns might push teams for increased complexity; Steeper learning curve due to a handful of unique narratives (e.g., interceptors, guards, modules, and more); Highly opinionated

**Fastify**

Pros: Relatively simple and lean; mostly based on Node.js/JavaScript standards; relatively shallow learning curve; with its official plugins cover many application concerns though not as rich as Nest.js;

Cons: Younger than others and not as popular yet; smaller eco-system compared to express and Nest.js

**Koa**

Pros: When compared with express: it's Simpler and nimbler; modern API with async/await support; better performance

Cons: Covers a small subset of a typical application needs - leaves a handful of app concerns uncovered; Not as popular as express and Nest.js

**FeathersJS**

Pros: Between Nest.js and Express in terms of batteries-included. Can run on top of Koa or Express.  Almost all functionalities are optional, but comes with common capabilities like authentication, object validation, error-handling, etc..  Provides a unified, common abstraction layer over all DBs, so it is very useful if your application must talk to multiple DB engines or if you plan to transition from one DB to another in the future.  Has a CLI generator and rich plugin community.

Cons: Can be more powerful, but more complex than Koa or Express by itself.  Has some conventions around "hooks" and "resolvers" that, though they simply interact with a Koa/Express Request object, can still be confusing at first.  Does not have the bells and whistles of Nest.js.

### A brief choosing guide

**Prefer express.js when** - having an experienced architect onboard _and_ in a need to control the fine-grained pieces of the puzzle. In this circumstances, Koa is also a solid option with a more modern API than express but a much smaller eco-system

**Prefer Fastify when -** The app consists of reasonably-sized components/Microservices (i.e., not a huge monolith); for teams who have solid JavaScript & Node.js knowledge; when sticking to Node.js narratives and spirit is desirable

**Prefer Nest.js when** - It's desirable to design and code in OOP style; when the team is highly experienced with Java/Spring/Angular or similar; for large size app that can't be broken down (i.e. monolith) to autonomous component; for a team that lacks fundamental JavaScript/Node.js skills (not exclusively, this yet another consideration); when the decision-making overhead should be minimized; when the time to the first delivery is a critical factor

**Prefer FeathersJS when** - When your team is not focused on OOP and dependency injection, but needs more batteries-included than Express or Koa.  Useful for abstracting against multiple DB engines if your sub-apps talk to different domains with different DBs.  
