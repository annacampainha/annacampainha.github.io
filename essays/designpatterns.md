---

layout: essay

type: essay

title: Baking Some Design Patterns

date: 2020-12-02

labels:

- Software Engineering

- Design Patterns

- Javascript


---
## Quote of the Experience 
I have many favorite quotes that motivate me to do better. For experiencing Design Patterns it is quite different:
Baking is science for hungry people

I chose this quote because I just so happen to be baking dark chocolate chip cookies as I brainstormed and comprehended everything for Design Patterns. As I was making my cookies, I realized design patterns are very similar to a recipe. When someone thinks of a pattern, they most likely think of a swirl or a arithmetic sequence. In my case, I see it as a recipe. We have a goal in mind and there are guidelines that help us get to that end goal. Now, in software engineering, design patterns is reused solution like a template that is used to develop software. Recipes (especially Nestle Tollhouse Chocolate Chip Cookie recipe) can be modified by users which then results into a new recipes. Similarly, that’s how design patterns are for software. There are four different types of design patterns in software engineering which are commonly used. 
They are: 
Factory 
Singleton 
Observer 
MVC

Now I won’t go over all of them but I highly encourage familiarizing yourself with each one.

##  The gooey insides of the importance of Design Patterns
As a three and half year Computer Science student, I will be honest and say I have never heard of a design pattern in coding. This is new to me starting this semester. I understand why it is key to having a design pattern because of ultimately is the key to developing software. There are so many steps within a pattern though that you must be careful that it works as a whole. One part might be important to make the entire design work, but there are many other key elements that piece together the pattern. It’s like the flour to cookies, you need it to stick together however, other really important ingredients are the eggs and the butter. As I said, patterns need pieces that help it stick together. 

## Reality of finding the pattern in my code
As I said, design patterns are so new to me. As Dr. Johnson was explaining the different types, I was actually very overwhelmed like when I google “best choc chip cookie recipes” and 500 million show up on google. I never knew what we were coding in our homework and project were actually coding patterns. Luckily the meteor template outline everything for us where we noticed a pattern like publishing, then we could apply it. 
Here is an example of publishing: 
```
Meteor.publish(Comments.adminPublicationName, function () {
  if (this.userId && Roles.userIsInRole(this.userId, 'admin')) {
    return Comments.collection.find();
  }
  return this.ready();
});
```
It was not aparent to me that these *patterns* had actual names, but it makes sense. Every .jsx file we create is a recipe to be baked, it may end up messy or it may not but we have the pattern to keep intuitively in check. 

## My pattern 
In my group project, my group and I are working on a database that has many users within a system. All of the patterns are so similar to patterns listed above. I notice that the “Singleton” design pattern is an ideal pattern my group follows because when a user subscribes, they receive the collection of data that they are signing up for. Each collection we have, it has a core so song class that manages access to it. For example, our users are Athletes and their Athletic Trainer. The Athletic Trainer can publish records of the rehab their athlete received at their last visit. The trainer has access to choosing what they want to see on that page whether it’s old or new data or specific to what they are searching for that is for that single athlete. Everything corresponds to a profile. 

Here is the code. Admin is for the Athletic Trainers and user is for the Athletes:
```
 this.userPublicationName = `${this.name}.publication.user`;
    this.adminPublicationName = `${this.name}.publication.admin`;
```

## (Not So) Moral of my Quote of the Experience
Do more things, read far into them (if you are already not an over-analytical computer science nerd) and find a connection to whatever is going on in your life. You'd be surprised with how many patterns really exist in this world. Design Patterns are a necessity when devloping software.

And scientists should bake more cookies. 

<img class="ui massive image" src="../images/cookies.JPG">

