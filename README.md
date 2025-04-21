# ZLINE Notes with Jeanie

## Why work here

- I really like your company
- I like your tech stack with 7 years and python along 3 years of typescript
  - I can step in and rapidly pick up golang
  - I recently answered several questions on leetcode and this feels very natural
- Recently got married and want to establish my career in Reno
  - Want to work in person; missing the in person collaboration after
  working remote for so long

## Why leave my company

- Tired of working remote

## Quick

- Make connections on pictures on office

## Homework

- Top 10 technical interview questions
  - Rapid fire measurable responses replacing numbers with percents

## Interviewers

- Sowmya Kudva - Software Engineer
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

- Loren Parvin - Salesforce Developer
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

- Tim - Director of IT & Development

## Top 10 Tech Interview Questions

1. Explain the difference between Agile and Waterfall development methodologies.
Waterfall is a step by step system with 4 phases; design, development,
testing, deployment. There is no going back once a phase is done. For example
once the design is created, the team must start development. Agile is a more
flexible process where work is done in short sprints with continuous
feedback. Waterfall takes longer and is best for fixed-scope well defined
projects while agile is best for constantly evolving projects.

2. What are design patterns and why are they important?

Design patterns are well known methods for implementing application logic.
For example if we want to make system wide settings, we would use the
singleton pattern which has a table with one item in it.

3. Describe your preferred programming paradigm and why you chose it
My favorite programming paradigm is object oriented. Having functions for
each object helps a lot to keep your code organized.

4. Explain the concept of polymorphism with an example.

Polymorphism is like inheritance but with function overrides. For example you
would make an animal class and inherit this class for dog, cat, lion, etc.
Then you would override the speak function for each animal and have it print
something different. This allows you to write the same code for each class
and get the correct result.

5. What is Big O notation and why is it important in algorithm analysis?

Big O notation is the worst case analysis of time and space complexty for
algorithms and functions based on input size. Improving the worst case time
complexity is way more useful than improving the best case time complexity.
For example searching for an item in a sorted list will have a time
complexity of O(n) while a binary search would take O(logn).

6. How would you design a system to handle a large number of concurrent users?

I would use a relational database like postgres and create an async api using
python django, golang, rust axum, or asp dotnet core. I would handle database
changes with migrations so I can test changes on my localhost and a
development server so I can apply the migrations after testing and know it
will all work immediately. I would use reliable cloud architecture with AWS
or Azure to handle user auth and attach related data to the users in my
postgres instance. Along with this I would use a caching system like redis to
make api calls faster and put less pressure on the relational database.
Another important aspect to our large project is to use auto scaling with
load balancing. This can be done with ALB and Fargate with AWS or Container
Instances on Azure.

7. Describe a bug you found in your work and how you fixed it?

A recent bug we ran into was the password change flow with fedex emails. The
emails were working on my local mailpit system so I ran the django shell with
my code to send slightly different emails to my manager's fedex email. We
found the issue was having too many query parameters in the reset password
link and it triggered a spam filter for the fedex emailing system. After
finding the problem I updated the production server.

8. Explain the concept of inheritance in object oriented programming.

Inheritance is the ability to have the same variables and functions for a
child class. For example you can have coordinates x,y in one class and make a
child class with z for a 3d object. This way you don't need to define the 3d
object with x,y, and z. It can just inherit x and y from the 2d object.

9. What are the four pillars of object-oriented programming?

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

10. Describe a time you had to work on a complex project and how you approached it
  I had to create a user system for a swift frontend app with admin tools. I
started out by choosing a tech stack; django, postgres, and aws ec2. Nice now
we can parse massive pdf files to json objects and save them, but this is
extremely slow, so I upgraded the parsing tool to a rust program. Ok now we
have the basics but we notice problems that are hard to solve, so I made a
logging system that captures logs for each request. Nice, now we have run
into a new problem. The database isn't strong enough for this log
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

## Behavioral Interview Questions

1. Why do you want to work for X company?
  I really miss the in person collaboration of on site teams and want to be
  located in Reno.
2. Why do you want to leave your current/last company?

  I want to be part of a bigger team.

3. What are you looking for in your next role?

I'm looking to grow myself along with others.

4. Tell me about a time when you had a conflict with a co-worker.
5. Tell me about a time in which you had a conflict and needed to influence somebody else.
6. What project are you currently working on?
7. What is the most challenging aspect of your current project?
8. What was the most difficult bug that you fixed in the past 6 months?
9. How do you tackle challenges? Name a difficult challenge you faced while working on a project, how you overcame it, and what you learned.
10. What are you excited about?
11. What frustrates you?
12. Imagine it is your first day here at the company. What do you want to work on? What features would you improve on?
13. What are the most interesting projects you have worked on and how might they be relevant to this company's environment?
14. Tell me about a time you had a disagreement with your manager.
15. Talk about a project you are most passionate about, or one where you did your best work.
16. What does your best day of work look like?
17. What is something that you had to push for in your previous projects?
18. What is the most constructive feedback you have received in your career?
19. What is something you had to persevere at for multiple months?
20. Tell me about a time you met a tight deadline.
21. If this were your first annual review with our company, what would I be telling you right now?
22. Time management has become a necessary factor in productivity. Give an example of a time-management skill you've learned and applied at work.
23. Tell me about a problem you've had getting along with a work associate.
24. What aspects of your work are most often criticized?
25. How have you handled criticism of your work?
26. What strengths do you think are most important for your job position?
27. What words would your colleagues use to describe you?
28. What would you hope to achieve in the first six months after being hired?
29. Tell me why you will be a good fit for the position.
