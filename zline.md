# ZLINE

## Why work here

- I’m excited about ZLINE’s tech stack—I've got 7 years of Python and 3 years of TypeScript experience, and Go feels natural after working through problems on LeetCode.
- I recently got married and want to plant roots in Reno. I also really miss in-person collaboration after years of remote work.

## Why leave my company

- I’m looking for in-person collaboration and a more connected team environment.

## Quick

- Make connections on pictures on office

## Homework

- Top 10 technical interview questions
  - Rapid fire measurable responses replacing numbers with percents

## ZLINE Specific

### Big topics

#### Code Review

- Optimizations in space/time complexity
- Catch potential bugs
- Enhance code reusability

#### Solution Mapping

-

#### Bigger Picture Design

- Utilize the right cloud services for scalability
- Choose the right frameworks and languages
- Optimize database design and queries

#### Mock Pull Requests

- Spot edge cases
- Add comments

#### Integration with other Platforms

- CI/CD tools like github actions, AWS code commit,

### Interviewers

#### Sowmya Kudva - Software Engineer

- **Senior Software Engineer at Tesla** leading full stack development to
  improve factory software and production efficiency
- Proficient in **Angular**, **TypeScript**, and **Golang** for building
  modern UIs and robust REST APIs
- Delivered a **unified design library integration**, enhancing front-end
  consistency and innovation
- **Redesigned user interfaces** to improve usability and support
  high-quality manufacturing workflows
- Collaborated with cross-functional teams to build scalable, reliable
  software aligned with Tesla’s mission
- Passionate about **pushing technical boundaries** to drive impact in the
  automotive industry

#### Loren Parvin - Salesforce Developer

- **Salesforce Developer and Administrator** with expertise in process
  automation, platform integration, and system optimization
- Strong foundation in **Computer Science and Engineering** with a passion
  for solving complex, high-impact problems
- Experienced in both **declarative tools** and **custom code development**
  within the Salesforce ecosystem
- Skilled in **system administration**, **technical troubleshooting**, and
  platform scalability
- Blend of **technical proficiency** and **soft skills**, including
  collaboration, creativity, and adaptability
- Passionate team leader who enjoys mentoring and sharing knowledge with
  others
- Committed to making a positive impact in every role, both professionally
  and personally
- Open to **networking**, **sharing ideas**, and **exploring new
  opportunities**

#### Tim - Director of IT & Development

## Interview Questions

### Top 10 Tech Interview Questions

#### 1. Explain the difference between Agile and Waterfall development methodologies

Waterfall is a step by step system with 5 phases; design, development,
testing, deployment. There is no going back once a phase is done. For example
once the design is created, the team must start development. Agile is a more
flexible process where work is done in short sprints with continuous
feedback. Waterfall takes longer and is best for fixed-scope well defined
projects while agile is best for constantly evolving projects.

#### 2. What are design patterns and why are they important?

Design patterns are well known methods for implementing application logic.
For example if we want to make system wide settings, we would use the
singleton pattern which has a table with one item in it.

#### 3. Describe your preferred programming paradigm and why you chose it

I prefer object-oriented programming—organizing code around objects makes it easier to reason about and scale complex systems.

#### 4. Explain the concept of polymorphism with an example

Polymorphism is like inheritance but with function overrides. For example you
would make an animal class and inherit this class for dog, cat, lion, etc.
Then you would override the speak function for each animal and have it print
something different. This allows you to write the same code for each class
and get the correct result.

#### 5. What is Big O notation and why is it important in algorithm analysis?

Big O notation is the worst case analysis of time and space complexty for
algorithms and functions based on input size. Improving the worst case time
complexity is way more useful than improving the best case time complexity.
For example searching a sorted list linearly is O(n), but binary search improves that to O(log n).

#### 6. How would you design a system to handle a large number of concurrent users?

I would use a relational database like postgres and create an async api
using python django, golang, rust axum, or asp dotnet core. I would handle
database changes with migrations so I can test changes on my localhost and a
development server so I can apply the migrations after testing and know it
will all work immediately. I would use reliable cloud architecture with AWS
or Azure to handle user auth and attach related data to the users in my
postgres instance. Along with this I would use a caching system like redis
to make api calls faster and put less pressure on the relational database.
Another important aspect to our large project is to use auto scaling with
load balancing. This can be done with ALB and Fargate with AWS or Container
Instances on Azure.

### 7. Describe a bug you found in your work and how you fixed it?

A recent bug we ran into was the password change flow with fedex emails. The
emails were working on my local mailpit system so I ran the django shell with
my code to send slightly different emails to my manager's fedex email. We
found the issue was having too many query parameters in the reset password
link and it triggered a spam filter for the fedex emailing system. After
finding the problem I updated the production server.

#### 8. Explain the concept of inheritance in object oriented programming

Inheritance is the ability to have the same variables and functions for a
child class. For example you can have coordinates x,y in one class and make a
child class with z for a 3d object. This way you don't need to define the 3d
object with x,y, and z. It can just inherit x and y from the 2d object.

#### 9. What are the four pillars of object-oriented programming?

The 4 pillars of object-oriented programming include encapsulation,
abstraction, inheritance, and polymorphism. Encapsulation is the use of
getters and setters for classes to simplify updates on the object. For
example you might want to update the database with last updated for every
change. For example get might need to update a last accessed timestamp and
set might need to update a last updated timestamp. Abstraction means to
define functions without having them do anything yet. For example a heap
always needs push and pop functions. You can make an abstraction for compare
since it's not always clear what to compare. In golang, you build a struct
that implements and interface to do this. Inheritance is the ability to reuse
functions and variables from a parent class. Polymorphism is the ability to
override functions from the parent class. This is similar to abstraction,
except you have a base function.

#### 10. Describe a time you had to work on a complex project and how you approached it

I had to create a user system for a swift frontend app with admin tools. I
started out by choosing a tech stack; django, postgres, and aws ec2. Nice now
we can parse massive pdf files to json objects and save them, but this is
extremely slow, so I upgraded the parsing tool to a rust program. Ok now we
have the basics but we notice problems that are hard to solve, so I made
a logging system that captures logs for each request. Nice, now we have
run into a new problem. The database isn't strong enough for this log
integration, so we started using RDS to decrease the server load. Awesome,
now let's figure out how to increase the speed for static files using s3. The
solution in this case is to create an oidc server and integrate with aws
cognito. I've learned a ton from this project. Now that I am more experienced
with hands on problem solving with application growth, I would use more cloud
services like aws cognito or azure directories to put the user base in a
managed cloud service that integrates better with things like s3 or azure
blob storage. Along with this, I would make more use of serverless functions
and kubernetes/fargate/container instances. Another improvement I would make
is to use code commit so that programs can be built on specific architectures
in the cloud without bogging down servers.

### Behavioral Interview Questions

#### 1. Why do you want to work for X company?

ZLINE’s mix of local impact and technical depth really draws me in. I’m ready to contribute and grow onsite with a tight-knit team in Reno.

#### 2. Why do you want to leave your current/last company?

I want to be part of a bigger team.

#### 3. What are you looking for in your next role?

I'm looking to grow myself along with others.

#### 4. Tell me about a time when you had a conflict with a co-worker

My coworker wanted the server to manage s3 files. I thought this would
be inefficient so I quickly built implemented it on the development server
to prove it wouldn't work well. After this I researched aws cognito and
s3 buckets and found a secure way to use the cdn. The biggest necessity
was security.

#### 5. Tell me about a time in which you had a conflict and needed to influence

somebody else.

I ran into a problem when a coworker wanted the server to handle s3
files. I implemented it on the development server to provide numbers
about the negative performance impact it would have.

#### 6. What project are you currently working on?

I'm working on fedexcrew for flyingbytes. It takes the monthly pdf
files and converts it to a user interface calendar on swift apps.
I'm using django with aws tools for the server and working with frontend
swift developers.

#### 7. What is the most challenging aspect of your current project?

The most challenging aspect of my current project is devops because
there are a lot of ways to deploy the project. My favorite implementation
is simple git hooks, but I have an issue because one of our servers is
on arm architecture so it's very slow to build my rust parsing tool on my
local x86 platform. I'm transitioning to aws codebuild and eventually
fargate with load balancing.

#### 8. What was the most difficult bug that you fixed in the past 6 months?

Either complex regular expressions or getting timezones to work correctly
for our pdf parsing tool.

#### 9. How do you tackle challenges? Name a difficult challenge you faced while

working on a project, how you overcame it, and what you learned.

I talk with AI for a little bit to get some ideas, then research the
documentation on them. Then I try and try to make it work. I've learned
that too much AI actually makes it harder to solve problems.

#### 10. What are you excited about?

I'm excited to learn from people more experienced than me and show
cool ways to do stuff to others.

#### 11. What frustrates you?

I get frustrated with the deny first methodology of AWS. I get it
though. Security is very important. It's just annoying when I don't know
if something is working because I fail to understand the concept or
if there is a simple security problem.

#### 12. Imagine it is your first day here at the company. What do you want to work on? What features would you improve on?

I want to work on backend development. I will take my time getting familiar with the current codebase, figuring out how to make
it work on localhost. Then I want to work on API development.

#### 13. What are the most interesting projects you have worked on and how might they be relevant to this company's environment?

My favorite project every was a music bot for spotify. It would monitor
users and make a master playlist based on skips and full play throughs. This
shows experience with APIs by using the spotify API. My biggest project has
been fedexcrew for flyingbytes. I have had to make a full api, implement
testing, deploy swagger ui docs, structure postman for the team, scale the
project up, and work with a team. More cool projects I have done include
an algorithmic crypto trading bot and an AI chatbot using ollama for more
humorous responses in telegram group chats.

#### 14. Tell me about a time you had a disagreement with your manager

At Aerovironment, my manager wanted to use a for loop to find an index
and I was pretty upset because I wanted to use an indexed database.

#### 15. Talk about a project you are most passionate about, or one where you did your best work

My most passionate project is with flyingbytes since it allows me to pay my bills.

#### 16. What does your best day of work look like?

I get to wake up at 11am, get on my computer and only talk to coworkers
or work undisturbed until 4am.

#### 17. What is something that you had to push for in your previous projects?

Pushing for aws components to work. It's a big deal keeping things
cost effective, secure, and scalable.

#### 18. What is the most constructive feedback you have received in your career?

At Aerovironment, I was told to make things work then add security, but with fedexcrew I have had to adopt the
exact opposite philosophy which ends up making me understand a lot more.

#### 19. What is something you had to persevere at for multiple months?

The regex parser for flyingbytes. I had to create regular expressions that work across 100s of thousands of
trips while maintaining correct time zones.

#### 20. Tell me about a time you met a tight deadline

Told my team I needed a week. Delivered it in two days.

#### 21. If this were your first annual review with our company, what would I be telling you right now?

You’d say I picked things up fast, boosted team energy, and delivered high-quality code from day one.

#### 22. Time management has become a necessary factor in productivity. Give an example of a time-management skill you've learned and applied at work

Don't go down the rabbit hole. This is the most important time management skill. There's a million ways to do anything
and the most important thing is to do heavy research for an hour or two, then get to it lazer focused.

#### 23. Tell me about a problem you've had getting along with a work associate

This one co worker would always over explain things and it bugged me but I would get over it.

#### 24. What aspects of your work are most often criticized?

Going down the rabbit hole. I love to explore and learn as much as I possibly can and sometimes it slows me down.

#### 25. How have you handled criticism of your work?

I learn more in my freetime.

#### 26. What strengths do you think are most important for your job position?

The ability to get along with people. I'm a great developer and have a decent personality. I think
it will be really fun to work with like minded people.

#### 27. What words would your colleagues use to describe you?

Smart, driven, and easy to work with.

#### 28. What would you hope to achieve in the first six months after being hired?

Becoming a master at golang. It has a perfect balance of simplicity and performance. I've
done a lot in Rust and Python. Those two are the exact opposite and I'm excited to work with
something in the middle. I also want to become an expert at building scalable systems using
Azure. Finally, I want to get great at working with large teams.

#### 29. Tell me why you will be a good fit for the position

It's almost impossible to get me away from my IDE and I love this stuff. No matter where I am,
mind is on how I can make something or make something better.
