# Node Shop App

### This application was created as a study project for the *Node.js - The Complete Guide* course on Udemy and can be accessed *[here](https://shop-app-course.herokuapp.com/)*

This app utilizes the following technologies:
  - Express framework
  - MongoDB for noSQL database, with the proper implementation in node being made through the mongoose ODM
  - Since it's a server side rendering app, it also utilizes EJS as the templating engine
  - Express-session for handling the login/logout functionalities
  - Express-validator for server side validation in every form
  - Bcrypt package for encrypting personal data (the user's password in this case)
  - Csurf package for CSRF protection
  - Multer for handling the uploaded images (initialy, the app utilized URL for the images, but was changed to uploaded files for better data control)
  - Connect-flash for errors feedback for the users
  - Nodemailer and Mailtrap API for sending emails (used in the password changing functionality)
  - Pdfkit API for creating invoices to your ordered products
  - Stripe API for handling payments (though it isn't fully implemented and was added only for study purposes)
  - Compression package for improving perfomance through the compression of bigger files (as the EJS and CSS files)
  - Helmet package for improving security through the addition of security headers in the responses (unfortunately, i had to comment out the package because it was conflicting with my delete function, probably due the frontend javascript file i am using to handle my delete)
  - Morgan was also added for creation of my own SSL certification but, since i deployed in Heroku which already handle the implementation of these security protocols, i didn't actually used this package.

This was a really good (and fun) project to build and i managed to pratice lots of new knowledges with it. I was able to understand from the most basic parts
of a server creation (like middlewares, routes, controllers and views setup, MongoDB/Mongoose models, pagination through server side configuration, debugging of a wide range of tecnologies) to more advanced topics (like validation and secutity handling, third parties' API implementation,
headers setup, HTTP and HTTPS protocols, deploy setup).

### Some challenges in this project:
 
 Despite being a guided project, i still had to deal with a few unplanned bugs (probably due to different versions of some packages). Lots of CORS errors kept happening even though i had
 already set up ways to deal with it. Depreciated commands were also quite common. Some bugs due data conflict in the database (like setting new fields for the models and forgetting to delete the old data with the old model).
 Most of the time i had to spend a few minutes staring at my browser's console and responses, trying to analyze all that information. In the end, i think all this really helped me to understand these tecnologies even deeper.
 When you have to look for some answers and go to the depths of StackOverflow and Documentation you start to understand not only **why** i didn't worked, but also **how** it actually works.
 
 Bugs may be annoying but they sure helped me to really understand what i was doing (and what i **shouldn't** be doing)
