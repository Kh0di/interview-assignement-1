# Interview Assignment #1 - beginner

Interviewee will be tasked to create a simple, fully static web application using React, a CSS framework of choice and Typescript to either demonstrate their already obtained knowledge and skill in front-end web development or their ability to adapt to and learn new things if this is their first project.

## General information

**Recommended for:** Complete beginners

**Difficulty:** Beginner

**Estimated time:** 1 week (5 workdays)

**Technical stack FE:**
  - React
  - CSS framework - either decided by the interviewer or interviewee can decide themselves
    - can be one of the following: Tailwind CSS, Material UI, Bootstrap etc.
  - Typescript


**Technical stack BE:**
  - none - FE web-app is completely static

## Assignment

Create a simple, static E-shop web-app. The project has 2 pages (Products page & User Profile page) and 1 dialog (Log-in dialog).

### Products page
Page for showcasing different products, represented via cards in a grid layout, available for purchase. Since the page is static, you can create your own list of products, but make sure they don't repeat too often. Using an online random data generator is advised.

**Acceptance criteria:**
  - *infinite scroll* - an e-shop can contain hundreds of products and rendering them needs to be seamless and quick, therefore an infinite scroll feature is a must
    - the 1st initial page should be loaded automatically, then every consecutive one loads only once user scrolls to the 80% length of the page
    - each page should load 20 products each
  - *search* - ablity to quickly and effortlessly search through dozens/hundreds of entries is another must
    - search the products by their name
    - make sure to throttle the ammount of requests somehow
  - *sort* - ability to sort the products via their attributes
    - sort the products by their name - 2 options: alphabetical normal and alphabetical reversed order
    - sort the products by their price - 2 options: lowest to highest and highest to lowest
  - *add to favourites* - ability to mark a product as a favourite for easier future purchases
    - restricted to only logged-in users
  - *add to cart* - ability to add a product to user's cart for purchase
    - restricted to only logged-in users
  - *responsiveness* - page should be responsive on all devices (from phones, through tablets to desktops)

**Mock up**
![products-page-mockup](https://github.com/Kh0di/interview-assignement-1/blob/master/mockup%20-%20products%20page.png?raw=true)

### User Profile page

Page for showing the products a user marked as favourite or added to their cart split into tabs.

**Acceptance criteria:**
  - the page content is split between 2 tabs
    - *Favourites*
      - sort function - same as on Products page
      - search function - same as on Products page
      - remove from favourites - ability to remove a product from the list
    - *Cart*
      - sort function - same as on Products page
      - search function - same as on Products page
      - remove from cart - ability to remove a product from the list
      - a Checkout FAB (floating button) at the bottom right
  - *logout button* - ability to logout from the site
    - returns the user back to Product page
    - the list of favorites and cart should not be deleted upon logout and should be unique to each user

**Mock up**
![user-profile-page-mockup](https://github.com/Kh0di/interview-assignement-1/blob/master/mockup%20-%20profil%20page.png?raw=true)

### Log-in dialog

User should be able to log-in and either mark different products as favourites or put them into their cart.
User's are dynamic and created on the go - if a user with entered credentials does not exists, a new one is created and saved in local storage, if they do exist, they are logged in and their data loaded from the local storage. **Use email as a unique user indentification.**

**Acceptance criteria:**
  - *dialog* - must be a floating dialog / modal / pop up window that is rendered atop of other content with a background shadow - clicking on the background hides the dialog as well as clicking on the close button
    - dialog should be centered
  - *validation* - both inputs need to be validated after submiting the form
    - both are required
    - email must be a valid email
    - password must be at least 8 characters long, contain 1 upper and 1 lower case character, a number and a 
    - if the validation is not met, an error message needs to be shown below the invalid input in question
    - pressing enter should validate and submit the form

**Mock up**
![login-dialog-mockup](https://github.com/Kh0di/interview-assignement-1/blob/master/mockup%20-%20log%20in%20dialog.png?raw=true)

## Notes for Interviewer

**For interviewer's eyes only !**

This assignment was created for (mostly) fresh beginners who never coded before (or at least not a FE web-app) to determine how quickly they can pick up & learn a new technology, how organized they are, how quick (or slow) they are and last but not least, how much they actually care and/or if they have a potential.

Juniors tend to think that just because this is a interview assignment it doesn't need to look too presentable - this also affects how some write their code as well.

**Pay attention to the following:**
  - how much knowledge/experience do they claim to have prior to taking the assignment
    - are they a complete newbie or already knowledgable in some aspects ?
  - how long did the assignment take them to complete ?
    - were they too quick ? or too slow ?
  - how was their communication during the assignment period ?
    - did they understood the assignment ?
    - did they ask any questions ?
    - if they couldn't complete the assignment in time, did they communicated that ?
  - were all acceptance criteria completed ?
    - if not, how many were missed and why ?
  - how does the project's file structure/hierarchy look like ?
    - does it makes sense ?
    - is the whole app stuffed in 1 single file or split into reasonable chunks ?
  - how does the code look like ?
    - is it in Slovak ?
    - is it organized ?
    - is it readable ?
    - is there a lot of commented-out code ?
    - are there any comments ?
    - residual console.logs ?
    - how much of the "tutorial code" has been copied from the libraries they might have used ?
