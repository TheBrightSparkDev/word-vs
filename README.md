# [Word VS](http://word-vs.herokuapp.com/)

Link to site [Word VS](http://word-vs.herokuapp.com/)

Word Vs is basically wordle with friends you challenge your friends to guess your word very simple lots of fun.
The inspiration for this mostly came from the idea behind wordle one man wanted to challenge his wife everyday.
So with the app anyone can challenge anyone everyday or even more than once everyday!

<img src="static/images/responsive-readme-3.png" alt="image of the website on various devices to show responsiveness" width="100%">

desktop and background credit: [pixabay](https://pixabay.com/photos/apple-computer-desk-workspace-1868496/)

# Table of contents
1.  [User stories](#user_stories)
2.  [Features](#Features)
  - [Homepage](#homepage)
  - [Sign-in/Sign-up](#signin)
  - [Profile](#profile)
  - [Challenge a friend](#challenge_a_friend)
  - [Challenges page](#challenges_page)
  - [Sent challenges](#sent_challenges)
  - [Add friend](#add_friend)
  - [Game page](#game_page)
3.  [Wireframes](#wireframes)
  - [Interactive](#interactive)
4.  [Challenges](#challenges)
  - [How many game boxes?](#challenge1)
  - [Database troubles](#challenge2)
  - [Last guess gone!](#challenge3)
  - [Why won't you break?](#challenge4)
5.  [Technology used](#technology_used)
  - [Wireframes](#wireframes)
  - [Frameworks](#frameworks)
  - [Libraries](#libraries)
6.  [Features left to implement](#features-left-to-implement)
7.  [Manual testing](#testing)
  - [Homepage.html](#homepage.html)
  - [Signin.html](#signin.html)
  - [Signup.html](#signup.html)
  - [Profile.html](#profile.html)
  - [Sent_challenges.html](#sent-challenges.html)
  - [Add_friends.html](#add-friends.html)
  - [Add_words admin.html](#add-words-admin.html)
  - [Add_words.html](#add-words.html)
  - [Base.html](#base.html)
  - [Challenges.html](#challenges.html)
  - [Create_challenges.html](#create-challenges.html)
  - [Edit_challenges.html](#edit-challenges.html)
  - [Friend_picker.html](#friend-picker.html)
  - [Game.html](#game.html)
  - [Oops.html](#oops.html)
  - [404.html](#page-not-found)
8.  [Manual public testing](#manual-public-testing)
  - [Big bugs](#big-bugs)
  - [Daniel found](#daniel-found)
  - [Rachel found](#rachel-found)
  - [Sharron found](#sharron-found)
  - [Small bugs](#small-bugs)
  - [Rhi found](#rhi-found)
9.  [Automatic testing with jest](#I-despise-JSdom)
  - [Script.js](#script.js)
  - [Deleteitem.js](#deleteitem.js)
10. [Validator testing](#validator-testing)
11. [Unfixed-bugs](#unfixed-bugs)
12. [Deployment](#deployment)
13. [Credits](#credits)
14. [My to do list](#todolist)
15. [Notes for assessor](#notes-for-assessor)

# User stories <a name="user_stories">

## Features<a name="Features"></a>

__Main menu__<a name="homepage"></a>

 - The main menu contains a few links to sign in sign up or guest mode.
 - This allows people to sign up sign in or just try out the game to see if they like it

![homepage](static/images/homepage.PNG)

- __Sign in/sign up page__<a name="signin"></a>
 - Both pages are extremely similar one adds a new user to the database if they dont already exist the other
 checks username and password match an already existing user.
 - This is to allow users to get into the advanced features of the game like challenging friends and seeing challenges
 that hae been sent your way.

![Sign in](static/images/signin.PNG)
![Sign up](static/images/signup.PNG)

__Profile__<a name="profile"></a>

- This is the first page you see when youre logged in, it looks different based on whether youre logged in or not.
To users that are logged in it will display all the available options: challenges, sent challenges, challenge a friend 
and freeplay. For users that are logged in as guest the only option they will have is freeplay.
- Freeplay gives users the opportunity to try before they sign up if they arent sure about whether they will like the game.

![Profile](static/images/profile.PNG)

__Challenge a friend__<a name="challenge_a_friend"></a>

- This is where you go to send your friends a challenge the first page you get to when you click the link off the profile is a friend picker. You first choose what friend you want to send the challenge to. Then you set the challenge the word needs to be valid and part of my database I've gathered of 48000 + words. This stops people from using bad words and making up words as that would ruin the game. You can also add friends on the friend picker page by accepting requests that have been sent to you.

![Friend picker](static/images/friend-picker.PNG)
![Challenge set page](static/images/create-challenge.PNG)

__Challenges Page__<a name="challenges_page"></a>

- This is where you see challenges you've recieved from others.
- This allows users to complete challenges other users have sent them.

![Challenges](static/images/challenges.PNG)

__Sent challenges__<a name="sent_challenges"></a>

- This page allows you to view and edit challenges you've sent to others and see if the person managed to complete the challenge or fail.
- This allows a user to edit the challenge they've sent if they arent happy with the word they sent off origionally it however doesnt allow the word to be edited if the challenge has been started. You may also delete challenges sent aswell.

![Sent challenges](static/images/sent-challenges.PNG)

__Add friend__<a name="add_friend"></a>
  
- This is where users go to add friends. If youre only just signing in please feel free to add thebrightspark which is my profile and challenge me! 
- Users will be able to add eachother here. It only allows you to add users that exist.

![Add friend](static/images/add-friend.PNG)

__Game page__<a name="game_page"></a>

- This is the main game where users will guess the words and they will display above the inout line in a grid you only have six guesses so mak sure they are good ones! Once you hit the guess limit its game over.
- Users will be able to complete challenges their friends sent them here or complete the freeplay levels.

![Game page](static/images/game.PNG)

__Add words page__<a name="add_words_page"></a>

- This is where users will be able to make suggestions for new words access to this page is only available if you type in a word currently not on my database.
- Users will be able to return to what they were doing easily after suggesting a word.

![Add words page](static/images/add-words.PNG)

__Add words admin page__<a name="add_words_page"></a>

- This is where admin users will be able to push any suggested words to their database
- Users will benefit from this as the admin will only approve real words and filter out any bad or non existant words

![Add words admin page](static/images/admin-add-words.PNG)

__Profile admin page__<a name="add_words_page"></a>

- This is the admin version of the profile these are the only options an admin will have.
- This makes sure that admins dont get distracted by challenges and its also impossible to add a admin.

![admin profile page](static/images/admin-profile.PNG)

# Wireframes<a name="wireframes"></a>

### Adobe XD<a name="interactive"></a>

[interactive wireframe](https://xd.adobe.com/view/2e9841de-1df7-47ef-b4e9-515a7a005f1c-7bcb/)

This is the best way other than using the site to get an idea of how everything works. There are no other wireframes created for this app as I went straight to a digital wireframe.

# Challenges overcome <a name="challenges"></a>

## How many game boxes??<a name="challenge1"></a>

### Goal

Displaying the correct amount of boxes on the game screen and the guesses to display and change the box background if the letter was in the right spot

### Issue

The correct amount of boxes relies on the html page knowing how many letters are in the word getting that info wasnt straight forward initially as I had no idea how to do it. 

It also relied on the html page knowing that the letter was in the right place and what the correct answer was without displaying it to the user

### How I did it

After looking back at previous mini project: task manager I noticed we used |length to find the length of a word which solved the first problem

next was the conditional formatting of the box it sits in the way I implemented this was by using loop.index0 to check the letters of both the guess and the answer match and then also used the in keyword in jinja to check if the letter was part of the word string. If the letter was in the correct place it adds the class correct if not it moves on to checking if its in the word if it is a letter included in the word it adds the class nearly otherwise it just displays the same color as normal.

## Database troubles<a name="challenge2"></a>

### Goal

To get the words onto the database

### Issue

I had a dictionary of 100k plus words varying in length and some even inclding special characters like "-" so the goal was to filter those out and only send over words between 5-8 letters long.

I didnt have time to do this manually

### How I did it

I created an app to iterate over the 100k words filter out any that include "-" and only send over the words if the length is '>' 4 and '<' 9 it took about 30 mins but when it was done I had 48k words and their definitions added to the mongo db database.

## Last guess gone!<a name="challenge3"></a>

### Goal

get the page to display the guesses correctly

### Issue

Upon submit the HTML page refreshes this causes the page to rebuild and send off the info at the same time...
problem here is that the system requests the info down from the server which at this point hasnt recieved the new guess so the new guess isnt displayed... 

I submit the form using javascript and the refreshing of the page means I dont need to clear all the input boxes which is ideal. Saves me creating an extra function and am not aware of a way of sending info from a html page to python without submitting

Also upon manual refreshing it sends the same guess through again which means refreshing the page again after a second delay is not an option

### How I did it

I sent the guess back to the HTML page via python I had to first of all add some if statements to check if any of the guesses had already been guessed then I would create a new dict that included the guess at the correct line. 

There is a small bug left here though if you manage to guess twice in less than 500ms it can cause and issue where the first guess is lost but doing this is very difficult and extremely unlikely.

I also got the python app to check if the guess had already been guessed and blocked it if it had. 
This lead to a lengthy function but it worked so thats all that mattered.

## Why won't you break!<a name="challenge4"></a>

### Goal

get keyboard to stop functioning after the correct answer was submitted

### Issue

I have to kill to javascript functions in order to do this but javascript is unaware what the correct answer is so I cant just check to see if the correct answer is displayed

### How I did it

Theory: If I add some condtional formatting to the html form to check if challenge.word == challenge.guess then I should be able to add an attribute to something so java knows if the correct answer has been guessed to use this to destroy the keyboard functionality I could set currentInputBox to a word string like completed then incrementing it or decreasing it by 1 would be impossible and therefore stop the game working and most importantly stopping the user submitting more answers and triggerring a gameover event by accident.

Theory above was absolutely correct and works perfectly.

# Technology used<a name="technology_used"></a>
## Wireframes<a name="wireframes"></a>
- adobe XD
## Frameworks<a name="frameworks"></a>
- I used the Flask framework to deliver the app using it's templating abilities it wouldn't have been possible without it.
- I used github to store the repository and version management
- I used gitpod for editing the code and for posting to github 
## Libraries<a name="libraries"></a>
- no libraries used

### Features Left to Implement<a name="features-left-to-implement"></a>

- free play mode

## Manual testing <a name="testing"></a>

### Homepage.html <a name="homepage.html"></a>

The correct function is just a page for users to decide if they need to sign in or out has no other functionality other than that.

#### Test cases

- Links to check
  - sign in, sign up and guest mode

### Signin.html <a name="signin.html"></a>

The correct function for this site is to allow the user to sign in if the user doesn't have log ins then there is a link to go to the signup page

#### Test cases

- Links to check
  - word vs links to the homepage
  - signup page
- The page should allow only users with extisting account to log in.
- If the user doesnt exist it will redirect users to the sign up page
- If the user exists it will allow them to log in if the password is incorrect 
- The flash message should display the same message regardless of whether the password or the log in is incorrect

### Signup.html <a name="signup.html"></a>

- The function of this page is to allow users to signup it doesnt differ much from the sign in page apart from the link at the bottom of the page is slightly different so the test cases are the same

#### Test cases

- Links to check
  - word vs links to the homepage
  - signup page
- The page should allow only users without an extisting account to log in.
- If the user does exist it will redirect users to the sign in page
- Once the user submits it should load the profile page
- The flash message should display the same message regardless of whether the password or the log in is incorrect

### Profile.html <a name="profile.html"></a>

- Usual functionality would be to display three different versions of itself one version for logged in users, one version to users that chose the guest option and another for the admin.

#### Test cases

- Links to check 
  - Sent-challenges
  - Challenges
  - Challenge a friend
  - The word vs is also a link but links to profile
  - sign out - removes the user cookie and send user to the homepage

Ways to check all versions is to log in as admin/ a regular user and also clicking the guest option.

Unfortunately freeplay mode has not been added yet so that link is not active.

### Sent_challenges.html <a name="sent-challenges.html"></a>

Normal functionality of this site is only to allow logged in users to use this site. Once a logged in user logs in it uses the session cookie's content to determine what challenges will be displayed. It should only display challenges that have been sent out by the current user. There are 4 different states that can be seen on this page created, started, completed and quit

#### Test cases

- The links to check:
  - Back goes back to profile
  - Word vs links to profile
  - Each challenge has a link depending on it's state
  - Completed and quit have links to delete
  - Created challenges have a link to edit the challenge.
  - Started challenges shouldn't have any links.

### Add_friends.html <a name="add-friends.html"></a>

Normal functionality of this page would be for a logged in user only to be able to add users that exist adding a user that doesnt exist should not be possible.

#### Test cases

- Links to check
  - add friend
  - back

The add friends button is a sumbit and it sends the username value to python to be checked if that user exists within the MongoDB database. This will display an error message if you add someone that doesnt exist.    

### Add_words_admin.html <a name="add-words-admin.html"></a>

This page should not be accessible to regular users only one account has access to this so testing is impossible outside of development.
Regardless one way it can still be tested is by trying to access the page. Usual functionality would be to display all of the suggstions that users have made and allow you to accept them.

#### Test cases

- links to check
  - Word VS takes you back to the admin homepage
  - Send button sends a suggestion to the mongoDB

The normal functionality is to send the word and definition from the word suggestion database to the word database. You can also add to the word or description currently there is no way to delete the suggestion other than on mongoDB currently so thats not a bug it's just yet to be implemented.

### Add_words.html <a name="add-words.html"></a>

Normal functionality should be that this page should only be accessible by logged in users the users. The link to this page should only display when the user inputs a word that doesn't exist on either the challenge creation page or the game page. Depending on where you came from the back button will send you exactly where you came from. This is my way of making it easier for people to help out in developing the word base.

#### Test cases

- links to check
  - Word vs should take you to the profile page
  - The back button should take you back where you came from.


### Base.html <a name="base.html"></a>

This simply acts as a placeholder for the content of each site it also holds the links to the css file it doesn't do an awful lot sadly and cant really be visualised apart from the background because that technically does come from the base

#### Test cases
- Best way to test if the base is displaying and working correctly is if the content is centered on the screen.
- Another way of checking it works is if anything on the screen has a style.
- The third of many other ways of checking is if the background is coloured blue and black in a linear gradient.
- It is very obvious if it's not working or displaying correctly

### Challenges.html <a name="challenges.html"></a>

Usual behaviour is to display challenges that the current user has been sent by their friends. It displays differently depending on the state of the challenge. If the state is created it will go into the New challenges box. As soon as the challenge is started the challenge state changes to started. While the state is started the challenge goes into the already started box. The reason they are seperated is because the started state allows you to give up on the challenge. Whereas the challenges that haven't been attempted cannot be given up on. 

#### Test cases

- links to test
  - Each challenge when clicked should take you to the game page for that particular challenge
  - Each challenge when started should allow you to press on a give up button. The give up button will remove the challenge from the list and the person who sent the challenge will be able to see you gave up or "quit" 
  - The word vs title should take you back to the profile.
  - The back button should also take you to the profile page.

- Try accessing the page while not logged in it should send you to oops.html
- Try to access a challenge that is currently being edited by the creator of the challenge it should stop the user from clicking on it.

### Create_challenges.html <a name="create-challenges.html"></a>

Usual behaviour is to allow a user to send a challenge. Each create challenge page will be for a specific user. If there is no user selected the page will go through to the 404 page. If the user isn't in the database for example if you changed the name at the top of the page after create_challenges then it would send users to the oops.html page with a custom message. This is caught by a try except catch which if it is unable to find the user instead of crashing and saying it doesn't have a get method it instead displays the oops.html page.

#### Test cases

- links to check
  - Send will send the challenge if the word is valid if not it will tell the user the word is invalid and give them the option to suggest the word
  - Back will go back to the friends list
  - word vs will as usual send you back to the profile page.

- Another way to try and challenge the page is to change the name in the web address to something different, change the name to a user thats not on the current users friends list and lastly removing the name altogether. The first two will give you oops.html the third will send you to 404.html.
- The last way to test the page is to click the link to suggest a word then on that page press back and it should send you back to create_challenge with the correct name in the address and any challenges sent should go to the intended user.

### Edit_challenges.html <a name="edit-challenges.html"></a>

usual behaviour would be to allow users to edit the challenge they sent their friend is maybe theyve changes their mind about the letters they want to send their friend or the word itself. There are some restrictions on what you can edit though. If the friend has already started the challenge then the person who made the challenge will be unable to edit it. 

#### Test cases

- links to check
  - the word vs title will as usual send you back to the profile page
  - back will send you back to the sent challenges page 
  - send will update the the challenge

- other ways to check is to see if you can access without being logged in
- to see if you can edit a challenge that has already been started
- to see if you can edit a challenge with a word that isn't valid or with letters that dont have the words letters in it 

### Friend_picker.html <a name="friend-picker.html"></a>

usual behaviour for the friend picker page would be a list of friends you have previously added all with links that take you through to create a challenge. Underneath this is another section called requests. Adding one of these will add them to your friends list. The way the computer differentiates the two lists is it checks friends on your friends list first which is the friendslist it then checks other users that have your name mentioned on their friends list but arent present on yours. The other usual behaviour of this page is to have a link to add new friends to your friends list 

#### Test cases

- links to check 
  - add friends link should take you to the add friends page 
  - each friend should when clicked take you to the create challenge page 
  - each request link will have a link to add the request clicking this will add them to your friendslist.
  - back should take you to the profile page
  - word vs title will take you as usual to the profile page

### Game.html <a name="game.html"></a>

Usual behaviour of this page would be to display a challenge you clicked on. It should then allow you to see previous guesses if any and also allow you to make new guesses. The page should only allow you (if using a keyboard) to type valid letters. It should also only allow valid word guesses if the guess is invalid it should allow the user to suggest a word. Upon clicking that link the back button should take you back to the game page with all progress saved. Upon making a successful guess the word should be added to the next available guess line in the guess box starting at the top. It should also conditionally format the background of the box the letter is in depending on the accuracy of the letter. Green means the letter is correct and in the correct place. Yellow means the letter is correct but in the wrong place. No colour means that the letter is not in the word at all. This also affects the keyboard as the keyboard will now display which letters are in the word which havent been tried and which have been tried and are incorrect. Making future guesses easier. The system will not allow repeat guesses and if the correct guess is made only the back button works from then on. Stopping users from guessing more and more and then losing due to the guesses running out. If the guesses run out the game will display a game over message and only back will work again. There is alot of logic when it comes to this page so I would suggest being creative to try and beat it.

#### Test cases

- links to test
  - back takes you back to the challenges page.
  - suggest word should take you to the add words page and push through the referring page so when you press back on that page it should take you back to the challenge you were just on with all progress saved.

- Other ways to try and break the page is to create a macro that types two words very quickly and see if you can force it to miss a word. I found typing 4 words in a second tends to miss the two middle words regularly. I don't see this as a bug though due to the fact that requires a typing speed of 173 words per minute the average . At a type speed of 172 words per second the system is able to pick up every letter at least on my testing runs.
- Try to enter an invalid word
- Try to access a challenge that's not for you
- Try to access a challenge that's been given up on 
- Try to access a challenge that has been completed or game over (this technically should still be possible but you should not be able to make any further guesses)


### Oops.html <a name="oops.html"></a>

Usual behaviour is to display what went wrong and how to fix it with relevant links 

#### Test cases

- links to test
  - home - displays if you tried accessing something that wasnt meant for yourself (if youre logged in it will take you to profile if you're not logged in you'll be sent to the homepage)
  - sign in - displays if youre trying to do something while not logged in
  - sign up - displays if youre trying to do something while not logged in
  - back - only displays if error occurs trying to challenge a friend thats not on your friends list

### 404.html <a name="page-not-found"></a>

The function of this page is to catch people who have manually typed in a bad address it has a link to the homepage and thats pretty much it 

#### Test cases

- Type in a bad link 
- Ff the 404 page displays then it's working correctly
- Click the link to see if it takes you to the homepage. 
- Due to the logic on the homepage backend if you are already logged in it will send you through to the profile page instead. 

# Manual public testing <a name="manual-public-testing"></a>

## Big bugs <a name="big-bugs"></a>

### I found <a name="daniel-found"></a>
 - The backspace doesn't delete the last letter on the currentWord variable which means the word either gets submmitted early after backspace or is a word that containns all the things you backspaced out the behaviour is only present in the keyboard controls and not the touch screen controls 
 - Bug was fixed by slicing currentWord (0,-1) which takes only the last letter off the word and reassigning the value to itself so currentWord = currentWord.slice(0,-1) 

### Bug tester Rachel <a name="rachel-found"></a>
 - found a bug where if you add a space to the end of the create challenge page it doesnt allow you to send and reason is unclear 
    - this has not been fixed due to time running out on the project
 - pointed out the rules are too small to see on a small screen
    - Text was made larger and more responsive

### Bug tester Sharron <a name="sharron-found"></a>
 - found a bug where you cannot add users that have a number in their name simply by creating a user name with a number in it that I couldnt add via app
  - removed validation rule to block numbers form add friends HTML page

## Small bugs <a name="small-bugs"></a>

### Bug tester Rhi found: <a name="rhi-found"></a>
 - Display bug on challenges page back and no challenges found were displaying badly on the page
   - corrected by making div responsive (flexbox) and centered the back button by removing a misplaced div end tag
 - Also spotted a spelling mistake on the add words page
   - characters was spelled charecters

# Automatic testing with Jest <a name="I-despise-jsdom"></a>

## Attention important notes to use JEST

- make sure you comment out the let length line in script.js for some reason (i'm yet to understand why) having this uncommented causes the test suite to fail I have made it very clear on the script.js and the script.test.js file what line it is. 

## Script.js <a name="script.js"></a>

Notes - These test were difficult to implement because the game is generated entirely using logic which meant that testing needed to run in the flask environment which is either impossible or not possible given my current experience. So I copy and pasted the page after it was built created a file called testgame.html and deleteitem.html used that to do my jest tests. Unfortunately I was coming across lots of issues. Code that works on the script and functions in manual testing was coming back as undefined in jest I'm still not sure why. The same with the code I have to comment out just to run a test. The javascript doesn't do much in terms of calculations and it all relies on info gathered from the dom which for some reason wasn't working correctly. So my biggest takings from my experience with jest is that it's not delightful at all. I can imagine it's great when all the tests dont rely on the dom. In Short I'm not fond of JSdom but jest is good for non html reliant javascript.

- Test 1
  - Check if dom is loaded - This was to make sure all other tests would be able to function theoretically. Unfortunately that's not the case because jest seems to do an awful job of mocking doms in my experience anyways.
- Test 2
  - Checks if the game locks up when game is complete - this was a difficult one to test as for some reason the jsdom was unable to view the elements as elements so getting the attribute from an element was impossible unless I was doing it inside the except tag which was confusing...
- Test 3
  - Tests if the system only accepts letters from the keyboard - This was impossible to test simply. For some reason no matter how many times you call the function in my script called letterspopulator() it doesn't change the value of the variable letters... Even though thats the only thing that function does so I had to manually enter the values. The function does work in manual tests and on heroku so I have no idea why it doesnt work on jest. Second issue was that I wanted to get the value of my currentWord after it had been edited by the clicked function but again no matter how many times I ran clicked it never edited the currentWord variable. So I had to create a new variable called currentWord and not bring the one in from my script which then worked.
- Test 4
  - check if backspace works after struggling through all the issues on the previous test I thought this would be easy to implement but unfortunately importing the backspace() function makes the dom check for a box with the id of (n) and delete it's content's which is obviously what backspace does but because jsdom doesnt recognise it as an element getting or trying to access its inner html is 'not a function' this meant I had to comment out that part of the backspace code to test that it was correctly editing the current word. All other tests where done manually to check the delighful way which is by using lots of console.logs in the script file.

## Deleteitem.js <a name="deleteitem.js"></a>
- Test 1
  - Check if dom is loaded - This was to make sure all other tests would be able to function theoretically. Unfortunately that's not the case because jest seems to do an awful job of mocking doms in my experience anyways.
- Test 2
  - Checks if the class tag hide is added - This was to make sure it was correctly toggling the hide element consider the fact that the item in question after adding a hide tag running the function to toggle the calsslist again which in a normal circumstance would remove the class hide doesnt actually do anything in jsdom. No matter how many times you call the function it just adds one hide class and never removes it. This makes further tests impossible using jest so the test to see if it removes the class was done manually.

# Validator Testing <a name="validator-testing"></a>

## HTML
 ### 404.html
  - No errors were returned when using the official [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fword-vs.herokuapp.com%2Fsent_challenge)
 ### Add_friends.html
  - No errors were returned when using the official [W3C validator](https://validator.w3.org/nu/?doc=http%3A%2F%2Fword-vs.herokuapp.com%2Fadd_friend)
 ### Add_words_admin.html
  - No errors were returned when using the official [W3C validator](https://validator.w3.org/nu/?doc=http%3A%2F%2Fword-vs.herokuapp.com%2Fadd_words_admin)
 ### Add_words.html
  - No errors were returned when using the official [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fword-vs.herokuapp.com%2Fadd_words_admin)
 ### Base.html
  - No errors were returned when using the official w3c validator all tests include the base.html so no direct link to this on its own.
 ### Challenges.html
  - No errors were returned when using the official [W3C validator](https://validator.w3.org/nu/?doc=http%3A%2F%2Fword-vs.herokuapp.com%2Fchallenges)
 ### Create_challenge.html
  - No errors were returned when using the official [W3C validator](https://validator.w3.org/nu/?doc=http%3A%2F%2Fword-vs.herokuapp.com%2Fcreate_challenge%2Fstuart)
 ### Edit_challenge.html
  - No errors were returned when using the official [W3C validator]()
 ### Friend_picker.html
  - No errors were returned when using the official [W3C validator](https://validator.w3.org/nu/?doc=http%3A%2F%2Fword-vs.herokuapp.com%2Ffriend_picker)
 ### Game.html
  - No errors were returned when using the official [W3C validator](https://validator.w3.org/nu/?doc=http%3A%2F%2Fword-vs.herokuapp.com%2Fgame%2F6257ed0a29f7a799a025bcfa)
 ### Homepage.html
  - No errors were returned when using the official [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fword-vs.herokuapp.com%2F)
 ### Oops.html
  - No errors were returned when using the official [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fword-vs.herokuapp.com%2Fadd_words_admin) 
  - The link here says add_words_admin but it's just becuase I triggered the oops page from that link is all. You can see what I mean here [admin add words page](https://word-vs.herokuapp.com/add_words_admin)
 ### Profile.html
  - No errors were returned when using the official [W3C validator](https://validator.w3.org/nu/?doc=http%3A%2F%2Fword-vs.herokuapp.com%2Fprofile%2F%3Fusername%3Dstuart)
 ### Sent_challenges.html
  - No errors were returned when using the official [W3C validator](https://validator.w3.org/nu/?doc=http%3A%2F%2Fword-vs.herokuapp.com%2Fsent_challenges)
 ### Signin.html
  - No errors were returned when using the official [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fword-vs.herokuapp.com%2Fsignin)
 ### Signup.html
  - No errors were returned when using the official [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fword-vs.herokuapp.com%2Fsignup)
# CSS
 ### Style.css
  - No errors were found when using the official [(Jigsaw) validator](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fword-vs.herokuapp.com%2F&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en)
# JS
 ### Script.js
 - No errors were found [JShint validator](https://jshint.com/) however two warnings were found neither of which I'm concerned about.
 ### Deleteitem.js
 - No errors were found [JShint validator](https://jshint.com/)

# Unfixed Bugs <a name="unfixed-bugs"></a>

 - Adding a space after a word in create challenges can cause confusion.
   - Ran out of time to implement a fix sadly
 - word_check is assigned but never used x 6
   - This is not a bug but worth mentioning as python insists it is the word_check variable is used to throw an error if it fails indicating the word doesnt exist in the database that is it's use.
 - env imported but never used 
   - This is also not a bug but again mentioning it as its in both python files it allows me to pull info from my env.py file things like the mongo database name and admin name
 - Using open without explicitly specifying an encoding 
   - I probably could've fixed this but didn't I would just need to look into how it needs to be encoded and specify that which is really quite an easy fix.

# Deployment <a name="deployment"></a>

I was using github as the repository for the whole project so when I wanted to create a live page it was very easy to do.

- The site was deployed to Heroku. The steps to deploy are as follows:


## How to clone repository:
 - Go to my github repository [Word VS](https://github.com/TheBrightSparkDev/word-vs)
 -  Click the code option and then copy the link
 - if you have git installed on your pc you can use git clone followed by the URL 

## How to deploy to heroku:
- To deploy to heroku you need to do the following 
1. Go to heroku create an account or sign in 
2. Create an app
3. Go to the deploy tab
4. Choose your preferred method
5. Choose the repository and deploy.
6. Things you'll need to do to ensure your system deploys correctly is: 
7. Create a procfile containing the following text: 
   - web: python app.py
8. Create a requirements.txt with the following content:
   - click==8.0.4
   - dnspython==2.2.0
   - Flask==2.0.3
   - Flask-PyMongo==2.3.0
   - itsdangerous==2.1.0
   - pymongo==4.0.1
   - Werkzeug==2.0.3
 9. Go to the settings tab now 
 10. Reveal config vars 
  - You'll need to add your own values to the following keys I can't for security purposes declare what mine are I will type the Key followed by a description of what it is.
    - ADMIN_REAL = The Value of this will be the administrator account. This is important for the add_words_admin page but not essential
    - IP = 0.0.0.0 (ACTUAL VALUE)
    - MONGO_DBNAME = name of the mongo db collection that holds the data
    - MONGO_URI = This is from the connect to python app tab on MONGODB site it will give you a link this is where to put that link
    - PORT = 5000 (ACTUAL VALUE)
    - SECRET_KEY = This allows you to display the flashed messages. For exmple the message that pops up when you type in a wrong password is a flashed message. the value can be whatever you like
11. for this app to work correctly you'll also have to follow my database setup 
inside your collection you should have 
- users
- challenges
- new_words
- wordlist 

12. (optional) wordlist should have the following keys (if adding your own word database)
- word
- meaning
- If not feel free to use the filter.py in the repository make sure youre database is setup first it will run for a good half an hour and is difficult to stop.

## The live link can be found here - [Word Vs](http://word-vs.herokuapp.com/)


# Credits <a name="credits"></a>

Below are the sources of all the media and content 

Backspace button image created by me using adobe illustrator.

## Almost no parts of the code on this website are copy and pasted 

- If I was struggling with anything I would simply go to website that I have linked below and read up on how to use the specific code and then I would simply use the code correctly. 

## Websites I copy and pasted from:
  - [google fonts](https://fonts.google.com/)
## All websites used are linked below nothing was copy and pasted just checked:

  - [Werkzeug security](https://werkzeug.palletsprojects.com/en/2.0.x/utils/)
  - [Jinja cheatsheet](https://jinja.palletsprojects.com/en/3.0.x/templates/#variables)
  - [Converting cursor to dict](https://stackoverflow.com/questions/28968660/how-to-convert-a-pymongo-cursor-cursor-into-a-dict)
  - [How to add item to dict python](https://www.w3schools.com/python/python_dictionaries_add.asp)
  - [Best way to make responsive text](https://www.w3schools.com/howto/howto_css_responsive_text.asp)
  - [Changing the value of a form element](https://www.w3schools.com/howto/howto_css_responsive_text.asp)
  - [How to get length of cursor](https://stackoverflow.com/questions/35692719/how-to-get-the-length-of-a-cursor-from-mongodb-using-python)
  - [How to use try except in python3 correctly](https://www.flake8rules.com/rules/E722.html)
  - [How to correctly use the hidden attribute](https://www.w3schools.com/tags/att_hidden.asp)
- Code Institute mentor also sent me a link to a template of a README.md to create a structure I changed everything and kept structure apart from the steps to deploy as there isn't anything to change added a bit about making sure it was root as docs brings up an error message for me saying failed to build.

## Content 

- No content was used form external sources

## Media

- No media was used from external sources the backspace.png was created by me in illustrator

# More coming soon! 
 
## Follow me on github to stay upto date and message me for project ideas/pitches always ready to work with someone.
 
# To do <a name="Todolist"></a>
 only started noting things when I noticed I started forgetting things
## Completed
  - make sure all pages go somewhere relevent when the title is clicked if title is present
  - create challenge needs to check if word is a word and if it is prevent it being sent
  - create challenge needs to make sure all the letters from the word are in letters
  - create challenge needs to make sure that all letters are unique
  - need to deploy page to heroku
  - user cant add self
  - user cant add user that doesnt exist
  - usernames are stored as lowercase only
  - cant use uppercase in username
  - add word page needs to be created needs to send words to a suggestion database also needs to check if word exists or not
  - add words admin needs to be created need to be able to see all suggestions and definitions and one click add to the wordlist database
  - delete function needs to be made for previous challenges page
  - edit function needs to be made for previous challenges page 
  - edit page also needs to change state to being updated but somehow revert it if the user cancels
  - need to make sure noone other than admin can get into the admin page
  - The only page an admin has easy access to is the add words and add words admin page
  - change test cases on readme to this format:
   - how it should work 
   - how you can push it to see if it breaks 
  - How to deploy via Heroku instructions including what variables you need to mention (not their values)
## Not done yet
- change code comments to this format
  - [Correct code docstring formats](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html)
   - Reason I didn't do this is because the way the Python file is currently commented is alot easier to read than a docstring format although I did go through and add a general description to everyfile in a similar format to a docstring
- freeplay mode
- words to note for potential freeplay levels
   - lashed
   - thyme
   - field
   - welded
   - phony
   - pushy
   - icycle
  
# Notes for assessor <a name="notes-for-assessor"></a>

# I have not used a sql database because when I started this project 27 days ago I was able to choose what sort of database to use

 - Personal reasons as to my I didnt want to use a sql database 
   - On this course the only sql database I was able to learn about was using a google api to communicate with a sheets document. This means having an account that has a 90 day free trial with access to sheets entirely possible admittedly but the issue is after 90 days I have to pay per access and this app makes alot of connections. I am aware there are other options but don't have time now after spending a month on this app to change it right at the end.
   - I was more comfortable with mongoDB as this was covered in full with extensive tutorials on it during the program.
   - I am aware that mySQL is used more in big applications and so it would benefit me to have it as part of a future portfolio but I also have another milestone project to complete so implementing it there would show I am able to use noSQL and mySQL making me more valuable in my opinion. 
   - The initial document I got that contained majority of the words for my app used a noSQL setting.
   - I did end up using a relational sort of setup using MongoDB regardless by using the exact same setup for each user even if some parts where blank which is the same for challenges with each guess being blank by default but still present.

 ###  Things I was told to say by code institute to explain to the assessor why my project doesn't fit the NEW UPDATED CRITERIA:
   - For those who are at an advanced stage of development of their projects; and who have adopted the approach of using a non-SQL database platform to model all data we suggest, you add a note to your readme to demonstrate that you understand the design trade-off you are making and have an understanding of the mapping from one to another.  Please see the example note below.
   - In this case, I have modeled my relational database on a non-relational database system., MongoDB. I have used the Mongodb best practice and guidance used when migrating relational database platforms to non-relational database platforms as my guide in this case.  I have used the following mapping 
     - table => collection
     - row => document
     - column => field
     - relationships => linking and embedding documents
  
  - Personally I just want my work to be marked regardless of the database I have used as I have made a working application put my all into it and don't want this to be ruined by Code Institutes decision to suddenly change the marking criteria. It's also worth noting they promised a video to show how to migrate info which they have yet to deliver on coming up 2 weeks since saying they would do it at 4:30 on the day of releasing this news.

PS: Also sorry my readme is so long.

Assessor only: Please email me for log in details for admin account if required or follow instructions to clone and deploy to heroku and set the ADMIN_REAL key to an account of your choosing to see the admin page.
thebrightspark1@gmail.com
I will ask for proof you're an assessor.