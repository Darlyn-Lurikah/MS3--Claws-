<p><strong>Claws</strong> is a web application for everyone nail art lovers, from the very beginners looking for tips, to experienced tech wanting inspiration for their next set.</p>

<p>Having been borderline obessed with nails art for probably entirely too long, and with Covid starting a boom in self taught nail techs and hobbyists, the Claws applciation is an answer to what myself and many others wanted. A place soley for nail art that doesn't require digging through unwanted posts</p>

<p>With this application users can create and account to share and keep track of their posts, unshare those posts or simply browse what others have shared</p>

[View Claws live here](https://claws-website.herokuapp.com/)
<hr>

## UX 
### Project Aims
The main aim of **Claws** is to provide a web-based application, with a minimal, user friendly design, that allows users to create, search, share their sets, tips and talents.

For this project a full-stack website was required that allowed users to manage a common dataset using **HTML5**, **CSS3**, **JavaScript**, **Python**, **Flask** and **MongoDB**.


#### User Goals
The user is looking for:
- A database they can search to find nail art posts.
- A user-friendly data management system with **CRUD** conventions to:

    - Create a user account.
    - View their user information.
    - Update (Edit) their user account.
    - Delete their user account.

- An user-friendly dataset management system with **CRUD** conventions to:

    - Create posts.
    - View others posts.
    - Update (Edit) their posts.
    - Delete their posts.

- An simple and easy to naviage interface.

#### Developer Goals
The Developer wants to:

- Create a simple and easy to naviage application where the people who enjoy nail art can showcase their work or browse what others have done.
- Demonstrate their newly learned skills utilising in a variety of languages and libraries as well as a document database system.


### User Stories

**As a Non-Registered User, I want to:**

1. Intuitively find posts within the database.
2. View posts registed users created without needing an account
3. Navigate to Register page to start an account.

**As a Registered User, I want to:**

1. Log into my account to gain access to the full functionality of the site.
2. Navigate to my user profile to edit my profile information.
3. View my own post's dashboard to edit if I need to.
4. View my own post's dashboard to delete it if I no longer want it.
5. Navigate to my profile delete my account.
6. Navigate to my profile page to view my uploaded posts.
7. Navigate to an add posts page to upload a new post to the database. 

**As an Administrative Account holder, I want to:**

1. View all uploaded post's dashboard to edit as needed
2. View all recipe dashboard to delete recipe as needed.


### The Five Planes

The five developent planes allow create a structure for the planning through create stages of a project. 

<strong>1. <u>Strategy</u></strong>

**Why build the project?**
To create a space where people who share the same interests can: 
    - Search for nail art. 
    - Post nail art or tips.
    - Not have to be registered to view post making the site more inclusive.

**What are the user needs?**
Users will likely want to: 
- To browse 
- To create own posts 
- Edit own posts 
- Delete own posts
- Log In 
- Log Out
- Customise their profile 
- Delete thier profile 
- View posts 
- Save posts 


<strong>2. <u>Scope</u></strong>

**How will we address user needs?**

Each users need will have a corresponding page, navigation/and or link to the database. 

- To browse
  - Home page with search bar 
  - Home page doesn't need user to be registered 

- To create own posts 
  - Register page to keep all posts in account 
  - Add posts page 

- Edit own posts 
  - See user posts page
  - Edit posts page 

- Delete own posts
  - Delete posts page via edit posts so functionalities are easy to find

- Log In 
  - Log In page 

- Log Out
  - Log Out page 

- Customise their profile
  - Edit profile page 
  - Profile page to display changes  

- Delete their profile 
    Delete profile page via edit profile so functiionalities are easy to find

- View posts
  - Home page with all posts 
  - User profile with all user posts 
  - Post dashboard to view posts in a bigger format
   
- Save posts (future functionality)
  - Favourites page to keep posts user favourited 
  - Favourites button easily accessed in grid and standalone posts 

<strong>3. <u>Structure</u></strong>

<strong>4. <u>Skeleton</u></strong>

<strong>5. <u>Surface</u></strong>

<strong>Database schema</strong>

**Collections**
- Posts
  - ID - For targeting the post in queries 
  - Image - For post subject/imterest  
  - Post_caption - Users can give information with post image
  - Poster - Links post with the creator (user)

- Users 
  - ID - Allow develpoer and user to modify the database regarding the user holding a specific ID
  - Username - To find the user by 
  - Password - For security. Passord is hashed by Werkzeug 
  - Profile_img - Users can upload and image of their choice
  - Profile_bio - Users can share info about themselves

### Features 
This site allows users to upload, edit and delete posts. Users can customise their account with a profile picture and bio, both of which they can edit. In their profile page users can also delete their account along with all their posts. 

## Existing features 

- Search: 
   - Users can make non case sensitive search based on the title of the post in 

- Log In/Out: 
   - Logs registered users in and out of their sessions returning them to the privileges of unregistered users

- Register: 
   - Creates new user accout and allow them access to registered user functionality 

- Delete proflie: 
   - Deletes user profile and all user posts attached to user

- Create new posts: 
   - User can create a new post by uploading an image then addinga title and caption 

- Edit existing post: 
   - Users can edit their existing posts by changing the title, caption or image or all three

- Delete existing post:
   - Users can delete their posts permanently from their account subesquently the home page 

- Upload profile picture: 
   - Users can customise their profile by uploading an image and writing a bio

- Edit profile: 
   - Users can edit their profile page by uploading a new photo and/ or changing their bio

- Feedback: 
   - Flash messages indicate to user the folowing functionalities are completed or need to be: 
     - Wrong username/password
     - User already exists 
     - Logged in 
     - Logged out 
     - Registered 
     - Post added/edited/deleted
     - Profile edited/deleted


## Future features

- Favourites:
   - So users can save posts the like when so they don't lose them

- Commenting:
   - To make for a mor einteractive site. Users can give other users feedback, edit and delte their own comments

- Chats:
   - Users can keep in contact

- Password change:
   - So users can change their passwords in their accounts for an extra layer of security 

- Password rescue:
   - Email password rescue so users can reset their password if they forget  


### Issues and bugs

**Masonary layout**
I used a css masonry layout that is supported by Boostrap 5 with the help of the Masonry plugin. Occasionally on load, the cards will overlap. A quick refresh solves it, but it is worth noting. 
