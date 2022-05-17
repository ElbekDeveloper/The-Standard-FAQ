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

It's better to have clean commit history and to focus on one feature implementation at a time.This way, people can easily replicate your work, in the future, by looking at all the files you had to change to resolve an issue.

## 4. How to start contributing to a project?

Look at [How To Contribute to Open Source Community?](https://youtu.be/mR0N-QxZqYY?t=458)

## 5. How to do a Pull Request the right way ?

If possible the PR name should reflect an open issue's name. Be careful of case. All caps for the main category, and capitalized for the title (like a news article title), and separated by colon. Most of the time we want the issue, the commit and the PR to share the exact same name.
