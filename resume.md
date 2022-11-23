Ronald Crooy
============

Data:
 - Hometown:  **Geldrop (near Eindhoven)**
 - Country: **the Netherlands**
 - Birthyear:  **1982**
 - Preferred occupation: **software developer, entrepreneur**
 - Motto: **Strong opinions held weakly**
 - Highest education: **Computer science Master degree**
 - Philosophy/religion: **stoic, atheist**
 - LinkedIn: [in/racrooy](https://www.linkedin.com/in/racrooy/)


Who is Ronald?
-------

I love engineering, my specialty is software, but I love all types of engineering. 
Making things, figuring out how things work, thinking of solutions, debating about solutions, pairing up with others, 
but what I love about engineering mostly is the idea that we can take control and build solutions.

For me entrepeneurship is strongly tied to engineering, taking initiaitve, coming up a new idea, thinking creatively, not waiting for other to pick up tasks, these are all aspects that are as important for engineers as they are for entrepeneurs. 

In general I love activities in which I can find *flow*, like surfing, walking with the dog in the forest, cooking, researching or learning about things, these are all activities that I can easily lose myself in.

Finally I am a parent, for me that means that I can share my knowledge and experience, something which I gladly do with colleagues if they are open to it. It means practicing patience and stoicism, the ability to let go of negative emotions quickly and focus on the good things.

Education
---------

**Master, Computer Science**; Eindhoven University of Technology 2000-2008 

Thesis title:  *Cycle Time Prediction: When Will This Case Finally Be Finished?*

An adapted version, shorter and better written, was published in Lecture Notes in Computer Science, 2008, Volume 5331/2008, 319-336 · Jan 1, 2008
[Link](https://link.springer.com/chapter/10.1007/978-3-540-88871-0_22)

Experience
----------

**Withlocals: 9 years**

I co-founded Withlocals as the sole software developer, this means I build everything initially.
The first 2 years my technical co-workers were interns or freelancers, during this time our entire stack was built.
I had to focus on everything, maintain everything, define architecture, solve problems and as a founder I was also 
involved in strategic decisions.

Later as the company grew, we were able to hire fulltime developers, and my responsibilities only increased. I kept focussing on 
development of the platform, but now people management was added. Since we did not have children yet, I spent most of my time working.

After the series A, I gave up the CTO role in favor of the role of Chief Software Architect, which means I could go back to doing what I did inititally and leave the meetings with managers about management to others. During this time I could again spent 95% of 
my time programming, architecting and doing devops.

I've learned so much here, its going to get its own chapter further in this document.

**Volt, European Data team: 2 years**

As a volounteer for the political party Volt, i build a small PWA to track the distribution of posters for the German campaigns. The app was built on request, and is to this day a volounteer project of mine.


**Sioux Remote Solutions: 1.5 years**
*placed via Sioux Embedded Systems*

For 2 years I worked on a project that enabled connecting to machines remotely, with the purpose of gathering metrics, doing maintenance and taking control. My work involved programming in C++ and C#, and parsing lots of existing projects, documentation etc. The company did not keep developer for long as it was an in-house project of the parent company, as a result the quality of code and documention was required to be high to simplify hand-overs to new developers.

I learned how to work in a structured process, how to deal with large existing codebases that are not forever yours to maintain. Also I got to play with electronics, solder wires, connect computers to machines and visit machines on site, which was fun.

**ASML: 3 years**
*placed via Sioux Embedded Systems*

At ASML I started as young developer fresh out of University, I was mentored by a bunch of older engineers of every type of background. ASML employs a great number of different type of engineers, physicists, and mechanics, and my first desk was situated next to a think tank from whom I learned a lot about everything related to engineering. I tagged along my mentors as I walked the halls, drinked coffee with stakeholders, sat in many meetings above my paygrade as a fly on the wall.

I learned how to not just build what was asked for, but what was needed, by really listening to your stakeholder and trying to place yourself in their shoes. Also, in hindsight, I learned you dont need a process in a tiny development team with experienced developers, you can just iterate and build things while talking extensively to your users.


History of my Technical Experience
--------------------

At ASML I worked in PHP and Java, connecting many datasources into a single MySQL for reporting. The job was essentially to make complex down-drillable reports in Zend Framework (php) with the data that was imported hourly or daily from various sources. Essentially it was data-engineering before that name was popular.

At Sioux I worked in C# (with  SQL Server) for the backend part, and C++ with a entirely custom application for the client that was running on various types of machines. I also had my first experience with electronics here.

At Sioux I got a couple days training by Martin Odersky in 2012 (I think), after which I was itching to use it. At Withlocals I decided with Play framework it was a good choice (2013), together with Anorm+MySQL and Angular 1.x on coffeescript I build the MVP.
Later we ditched coffeescript for plain Javascript (ES6) with ReactJS. Coffeescript's whitespace significance was just too sensitive for errors, and I never liked Angular. Later we switched the fronted codebase to Typescript, which I can honestly say I love.

Over the years I learned how to properly use AWS/GCP, I started with manually managed EC2 Instances, moving to AWS Elastic Beandstalk, ending in a GKE kubernetes clusters with our infrastructure as templated-yaml in a git-repo. I learned many things about devops at Withlocals.

Our Scala codebase stayed for the most part in Play Framework, we upgraded Scala versions, ending in 2.13 with the planning to move to 3.x in the future. We added some extra separate projects (micro-ish services) in Akka-http, and lately one using ZIO. All in all Scala is at this point my preferred language if I would have to build a custom thing, I use it every year when I do the advent-of-code. 

Noteworty things I made/did
-----------------------

Big or small, these are things I remember vividly. I am omitting a lot of things I build over the last 9 years as founder, but these things I picked out due to noteworty-ness.

### Complex Syncing 
At ASML I build a synchronization which read XML files and imported them into a MYSQL. Every hour we checked what changed in an Oracle Database, comparing and filtering which files required reading. We then read the XML files, containing the bill of material (a tree with sub-components) of a single component and many more attributes.  On a daily basis we also pulled other details on components from SAP, thus combining multiple data sources.
The resulting trees with parts of the ASML machines, were then rolled up to simplify aggregation for a set of specific reports.

### Bugfix in C++ custom String implementation
I encountered, debugged, tracked down and fixed a bug in a custom String implementation in C++. The 
implementation had copy on write, and obviously the bug was related to multi-threading. This was in my early career, and this bug alone taught me the complexities of multi-threading and memory. Also I try not to use C++ if I can avoid it due to this experience.

### Event collector + tracker
I build, in a short week, a Akka-Http event collector + JS-tracker named Bitterbal to replace a large, complex and overly generic Snowplow setup. 
I stole the api-design (not the implementation) for the JS-tracker from the library for Segment, essentially sending events to multiple tools (GA, TrackJS, and more). Our own collecter simply parsed and validated the JSON that was POST'ed, and stored them in a Bigquery instance. The design is simple, but the tool was insanely efficient, never crashing, scaling when needed, we have not made a single change or bugfix after launch. 

### FP skills
Before ZIO existed, when we just started using ScalaZ, I implement our own version of the IO monad. Using a set of implicit classes and `ScalaZ's EitherT[Future, ErrorMessage, T]`, I made a easy to use and very fluent type called a `TaskResult`. Combining various nice helpers it made it very easy to chain async operations, flatmap/for-yield over their results and return things over an API. When I learned about ZIO, ofcourse I banged my head as I encountered the lack of an Environment type, but it proved too complex to add this feature and/or migrate to ZIO, so sadly we missed that part.

### Domain Driven Design
At some point when Withlocals was a success, when we felt confident in our business model and its value, we started looking at our architecture and organization from a Domain Driven Design perspective. This was a longer, on the side project, which proved to be a great guide for our architecture as a whole. It enabled us to define which things belonged in separate modules or not, it provided us with a structured way of discussing the architecture and organization as a whole. 

### Event sourcing magic
For V2 of our booking system, easily the most complex part, we implemented an event sourced version of the booking concept. A booking system is very little CRUD and most of the changes are result of important events like confirming a booking, finishing or starting payment etc. I learned the power of this system, but also that using this for CRUD things is probably not a great idea.

### Offline first PWA
For Volt I made an offline first PWA, the challenges here were mostly around deploying improvements or fixes. Once distributed, you have to make sure any future version of software can upgrade from this point without corrupting data. This proved to be probably the most complex part. Of course users used the app wrong, in unintend ways, so you have to make changes without breaking things. Especially this happens during an active campaign, making this volounteer work quite a bit more stressful.


Technology skills:
---------------
 - Javascript
 - Typescript
 - Coffeescript
 - Scala
 - ScalaZ
 - ZIO
 - Prometheus
 - SQL
 - Akka
 - Play Framework
 - MySQL
 - AWS
 - Google Cloud
 - Deno
 - Node
 - Python
 - Airflow
 - Bigquery
 - Angular 1.x
 - PHP Zend framework
 - NextJS
 - IPFS
 - RxDB
 - Postgraphile
 - Postgresql


CS Skills:
 - Domain Driven Design
 - Functional programming
 - Object Oriented Programming
 - Agile Scrum, Kanban
 - Waterfall
 - Data engineering
 - Mobile development (cordova, PWA)
 - Silent meetings


More details:
------------

Ideal working conditions:
- hybrid remote/office
- 4 day workweek
- flexible hours
- fun, social environment, very informal
- diverse team, I learned that a diverse team really enables original viewpoints
- silent meetings [Silent meeting manifesto](https://medium.com/swlh/the-silent-meeting-manifesto-v1-189e9e3487eb)
- zero tolerance for pointless loud meetings
- high tolerance for Dutch directness, bluntness and sarcasm

Family:
- 2 kids, girls
- wife
- dog
- chickens

Human Languages:
- English (fluent)
- Dutch (native)
- German (holiday sufficient)
- French (holiday sufficient)

Sports:
- Wave-Surfing
- Wind-Surfing
- Running (yogging through the woods without deadlines or goals)
- Pencak Silat
- Ashtanga Yoga

Hobbies: 
 - Walking (with the dog)
 - Learning/researching
 - DIY/Construction
 - Engineering
 - Coffee 
 - Cooking
 - Debating anything over a drink
 - Parenting

Most stupid mistakes I made:
 - working too many hours, too long days, and doing complex things on the way out at friday 18.00, thus making a stupid mistakes, like accidentally deleting the entire Elastic beanstalk environment causing all our servers to be removed. Although I managed to bring it all back in less than 30 minutes from backups, without any dataloss reported.
 - Picking MySQL when I could have just picked Postgres
 - Storing too much data in the frontend, or too much business logic for that matter.
 - Giving up a seat at the management table
