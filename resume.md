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

Where I worked
----------

### Withlocals: 9 years

I co-founded Withlocals as the sole software developer, this means I build everything initially.
The first 2 years my technical co-workers were interns or freelancers, during this time our entire stack was built.
I had to focus on everything, maintain everything, define architecture, solve problems and as a founder I was also
involved in strategic decisions.

Later as the company grew, we were able to hire fulltime developers, and my responsibilities only increased. I kept focussing on
development of the platform, but now people management was added. Since we did not have children yet, I spent most of my time working.

After the series A, I gave up the CTO role in favor of the role of Chief Software Architect, which means I could go back to doing what I did inititally and leave the meetings with managers about management to others. During this time I could again spent 95% of
my time programming, architecting and doing devops.

I've learned so much here, its going to get its own chapter further in this document.

### Volt, European Data team: 2 years

As a volounteer for the political party Volt, i build a small PWA to track the distribution of posters for the German campaigns. The app was built on request, and is to this day a volounteer project of mine.


### Sioux Remote Solutions: 1.5 years
*placed via Sioux Embedded Systems*

For 2 years I worked on a project that enabled connecting to machines remotely, with the purpose of gathering metrics, doing maintenance and taking control. My work involved programming in C++ and C#, and parsing lots of existing projects, documentation etc. The company did not keep developer for long as it was an in-house project of the parent company, as a result the quality of code and documention was required to be high to simplify hand-overs to new developers.

I learned how to work in a structured process, how to deal with large existing codebases that are not forever yours to maintain. Also I got to play with electronics, solder wires, connect computers to machines and visit machines on site, which was fun.

### ASML: 3 years
*placed via Sioux Embedded Systems*

At ASML I started as young developer fresh out of University, I was mentored by a bunch of older engineers of every type of background. ASML employs a great number of different type of engineers, physicists, and mechanics, and my first desk was situated next to a think tank from whom I learned a lot about everything related to engineering. I tagged along my mentors as I walked the halls, drinked coffee with stakeholders, sat in many meetings above my paygrade as a fly on the wall.

I learned how to not just build what was asked for, but what was needed, by really listening to your stakeholder and trying to place yourself in their shoes. Also, in hindsight, I learned you dont need a process in a tiny development team with experienced developers, you can just iterate and build things while talking extensively to your users.


History of my Technical Experience
--------------------

At ASML I worked in PHP and Java, connecting many datasources into a single MySQL for reporting. The job was essentially to make complex down-drillable reports in Zend Framework (php) with the data that was imported hourly or daily from various sources. Essentially it was data-engineering before that name was popular.

At Sioux I worked in C# (with  SQL Server) for the backend part, and C++ with a entirely custom application for the client that was running on various types of machines. I also had my first experience with electronics here.

At Sioux I got a couple days Scala training by Martin Odersky in 2012 (I think), after which I was itching to use it. At Withlocals (in 2013) I decided that Scala with Play framework was a good choice, together with Anorm+MySQL and Angular 1.x on coffeescript I build the MVP.
Later we ditched coffeescript for plain Javascript (ES6) with ReactJS. Coffeescript's whitespace significance was just too sensitive for errors, and I never liked Angular. Later we switched the fronted codebase to Typescript, which I can honestly say I love.

Over the years I learned how to properly use AWS/GCP, I started with manually managed EC2 Instances, moving to AWS Elastic Beandstalk, ending in a GKE kubernetes clusters with our infrastructure as templated-yaml in a git-repo. I learned many things about devops at Withlocals.

Our Scala codebase stayed for the most part in Play Framework, we upgraded Scala versions, ending in 2.13 with the planning to move to 3.x in the future. We added some extra separate projects (micro-ish services) in Akka-http, and lately one using ZIO. All in all Scala is at this point my preferred language if I would have to build a custom thing, I use it every year when I do the advent-of-code.

Noteworty projects
-----------------------

Big or small, these are things I remember vividly. I am omitting a lot of things I build over the last 9 years as founder, but these things I picked out due to noteworty-ness.

### 2008-2011 Data engineering pipeline
This was my first project after graduation. 

I helped built (from the beta MVP) up an internal information system at ASML that combined data scraped from SAP and Team-Center-Engineering. SAP contains business and logistical information on the production proceses, and TCE contains the engineering view on the production process.

The Cerberus information system combined those two views. The project was run like a startup, where we had to continuously find users, and adapt or expand our information system to satisfy users. My job was to gather requirements, iterate over a new feature and make sure it was running smoothly. I worked on the UI, the backend, and the database synchronization pipelines to scrape the data and combine it all. 

Skills: 
- PHP
- MySQL
- Java

### 2012 a Bugfix in C++ custom String implementation
I encountered, debugged, tracked down and fixed a bug in a custom String implementation in C++. The
implementation had copy on write, and obviously the bug was related to multi-threading. This was in my early career, and this bug alone taught me the complexities of multi-threading and memory. Also I try not to use C++ if I can avoid it due to this experience.

Skills: 
- C++

### 2012 connected a parkinglot-gate to the internet
As a project for Sioux Remote Solutions i had to connect a parkinglot-gate to the internet, it involved screwdrivers, soldering irons, c++, c# and a lot of learning about hardware.

Skills:
- C++
- C#
- electrical engineering

### 2013 Withlocals MVP
I helped build Withlocals as co-founder, fullstack-developer, CTO.

I started as the sole technical co-founder, and we hired freelancers and interns for frontend and design. All in all we build our MVP in 5 to 6 months. In hindsight we built way too many features in our MVP, but we did have a full booking system, admin system and a complete website with extensive search features, product catalogs, and various SEO and SEA solutions in place.

Skills:
- Team leading
- Scala
- MySQL
- AWS
- CSS
- JavaScript 
- CoffeeScript
- AngularJS
- CI/CD

### 2015 New cordova app 
We built our first cordova app in AngularJS with the help of some great interns, but after some lessons learned we rebuilt the app with a much different UI in ReactJS. 

Skills:
- Cordova
- PWA
- JavaScript
- React

### 2016 Withlocals Originals
After various iterations we decided to build a new product. The process involved a lot of planning, as it was a mix of sending out a team to Rome, Italy to improve our pictures, shoot videos and train our local guides in the new concept. 

My part was to modify our systems, guest facing, host facing and internal tooling as well as various core systems in our platform to make this work.
We built these features within the estimated time, cut some corners, but we successfully launched this pivot and we found product market fit.

Skills:
- Team leading
- Scala
- MySQL
- AWS
- CSS
- JavaScript 
- Reactjs

### 2017 Moving from AWS to GCP
Due to some funding we got from Google, we moved our entire stack from AWS to GCP in a matter of months.
We moved our stack from AWS Elastic Beanstalk to GPC GKE, with zero downtime due to the magic of mysql replication magic.

Skills:
- Kubernetes
- MySQL
- GCP
- AWS
- Scala
- Redis

### 2018 Pink is the new blue
A branding change, which started with a simple color change. The project started simple, but we expanded the project to also rewrite the frontend from angularjs to react. Which then got expanded so most pages got new designs. As projects go this one was a classic scoping problem, the scope got expanded constantly. 

However we succesfully rewrote and rebuild our entire frontend, with some good performance and usability improvements. In the end we managed to build the website in such a way that we also were able to deploy the whole frontend as a cordova app.

Skills:
- cordova
- Scala
- CSS
- Typescript
- Reactjs

### 2019 Group tours
We refactored a key part of our application, the booking system so we could support group tours. This involved splitting up one of our core domain entities into two 1-N domain entities.

Skills:
- Domain Driven Design
- MySQL
- Scala

### 2020 Data engineering
From a reporting system direclty on top of our MySQL db, to a full data pipeline using Airflow and bigquery.

Skills:
- MySQL
- Scala
- Python
- Airflow
- Bigquery

### 2021 Offline first PWA
For Volt I made an offline first PWA, the challenges here were mostly around deploying improvements or fixes. Once distributed, you have to make sure any future version of software can upgrade from this point without corrupting data. This proved to be probably the most complex part. Of course users used the app wrong, in unintend ways, so you have to make changes without breaking things. Especially this happens during an active campaign, making this volounteer work quite a bit more stressful.

Skills:
- PWA
- Postgres
- CSS
- Typescript
- Reactjs
- Offline first
- RXDB

### 2022 New Withlocals UI using NextJS

As a concept we created a brand new simple product- & checkout-page using an Api first SaaS webshop, Auth0 and Nextjs. We proved we could quickly setup a fully working replacement for the product page and checkout page while smoothly integrating with our existing Stack.
We had to create a couple new API's for our partner-api, as we integrated with ourselves as if we were a partner.

Skills:
- Auth0
- Typescript
- Reactjs
- Scala
- NextJS


Technology skills:
---------------

### Tools, languages, frameworks:

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
 - Jenkins
 - Kubernetes
 - Cordova

### CS Skills:

 - Domain Driven Design
 - Functional programming
 - Object Oriented Programming
 - Agile Scrum, Kanban
 - Waterfall
 - Data engineering
 - Mobile development (cordova, PWA)
 - Silent meetings
 - CI/CD


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
