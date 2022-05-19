# The-Standard-FAQ

## Vidéos:
<img width=20 src="https://www.searchmarketingaustralia.com.au/wp-content/uploads/2017/10/original_images_YouTube.png" /> [AMA001: Questions About The Standard](https://www.youtube.com/watch?v=1de5nMDj8Ys)

## 1. I was looking otripleS solution you are directly exposing  domain entities but in my development career I was using viewmodel or DTO’s can you explain us when to use ViewModel or DTO?

DTO approaches assume that the APIs are responsible for populating audit fields, ids ... etc.

But in reality there are scenarios where you want to let the consumer control these fields. Like a migration scenario for instance. You can't force maintaining certain audit fields like created and updated dates without Hacking into the database and by passing your API because of the DTO model.

## 2. How to name my branch for a PR?

### Branch Naming Convention:

users/[github-username]/[Issue-type/category]-[entity]-[action]

Look at this [video at the 25:10 mark](https://youtu.be/mR0N-QxZqYY?t=1510)

It helps you search branches and help you focus on one thing at a time.

<img src="https://user-images.githubusercontent.com/56794425/168654407-ce181cd6-8a6e-4ad8-b3c6-c7d44d476aac.png" width="50%" >


### Commit, Issue and PR naming convention:

Most of the time we want the issue, the commit and the PR to share the exact same name.

- DATA: Add RefugeeContact Model

- BROKERS: Insert Refugee

- CONTROLLER: POST Refugee


## 3. Why should I be careful with the commit history of my PR?

It's better to have a clean commit history and to focus on a single implementation at a time. This way, people can easily replicate your work, in the future, by looking at all the files you had to change to resolve an issue.

We asked Hassan Rezk Habib :

>Why should I be careful with the commit history of my PR?
>
>Hassan :
>I'm just using the commit history as a vehicle to establish 3 things. Three important things. 
>
>1. Logging or history of how a feature was implemented. 
>
>That commit history helps me know whether this code was actually test driven or not, right? There's no way you can actually determine that some code was written in a good quality, unless there is a commit history that says, "here's a failing test that we committed, and here's a passing test that made it past". 
>
>Okay now, any smart guy out there could hack it, right? 
>(...)
>Eventually you're going to get tired (...), because it makes you feel bad. You know you're cheating.
>
>So, I want to make sure of "How the code was written". 
>
>It is embedded and recorded in the pull request itself, including these very tiny break off sessions. I look at some of my team work and I say OK between 12:00 and 1:00, we actually split off to go have lunch and come back. 
>
>Someone else might be seeing just commits. I'm seeing a story of how that code came to be, so that's number one. It helps us know where the code came from and where it's going. 
>
>2. It establishes fairness. 
>
>What does that mean? 
>
>Sometimes you can't have more than one engineer creating the pull request. So, if it's only one engineer creating the pull request, there's no way I can tell who else contributed to that code. 
>
>This is how GitFyle (Hassan's web-app for GitHub stats) determines that you were pairing, that you contributed to foundation services, brokers, and all that kind of stuff, by looking at this commit history and seeing who else contributed to that. 
>
>There are a lot of smart engineers out there, that don't speak up for themselves. And then, there's this cowboy engineer that comes in, and says, "hey, let me just wrap it up and make the final commit", and then they take all the credit for the work. 
>
>That's not fair. 
>
>These engineers, the other engineers that are actually doing the hard work, they become invisible because there's no data that says, that they actually were a part of developing this awesome feature, so establishes its fairness in the world. 
>
>Now to the third thing. Which is the most important part.
>
>3. It plays as an educational tool. 
>
>How is that the case? 
>
>You want to know what it's like to write a failing test. 
>
>And what it's like to make it pass? 
>
>This will show you that.
>
>In fact, the commit history is more, much more, valuable than "The Standard" (Hassan's book on software engineering) Itself. 
>
>Because "The Standard" is just a bunch of ideas and theories, but the commit history is how these ideas come to life, and become living, breathing...you know... moments in your life that... I use the code to record... "This is me, recording a very precious moment"... in your life when you are changing the world. One line of code at a time.
>
>Does that make sense?

## 4. How to start contributing to a project?

Look at [How To Contribute to Open Source Community?](https://youtu.be/mR0N-QxZqYY?t=458)

## 5. How to do a Pull Request the right way ?

If possible the PR name should reflect an open issue's name. Be careful of case. All caps for the main category, and capitalized for the title (like a news article title), and separated by colon. Most of the time we want the issue, the commit and the PR to share the exact same name.
