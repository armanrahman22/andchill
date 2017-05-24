AndChill
======================================

This repository contains code for the AndChill application.

1. On some computers, the tests have trouble running. We were unable to pinpoint the exact cause of this problem. However, all the tests really do pass! We think the problem may have to do with the number of concurrent Mongo connections or the Mongo version. Allowing up to 100 concurrent connections on Mongo 2.6.6 works on Mac OS 10.9.5. Here's an image of the tests running: http://imgur.com/tHaU3yp

2. All the functionality covered by the tests has also been manually tested to be working on other systems. It appears the tests were written incompatibly with some systems.

3. We decided to divert from our original plan and show profile images to users before they accept a Chop. We're a dating app, and although mutual interest is important, attraction provides an additional spark.

README from our MVP
--------------------------------------

1. The project URL on Heroku is https://infinite-shelf-5577.herokuapp.com/. *However*, it is preferable to use http://andchill.co, because our Facebook login system is configured to use this domain.

2. To deploy locally, clone the code from Git, fire up MongoDB, and run `npm start`. Then, navigate to http://localhost:3000/ to explore the application. Facebook login will not work locally because it is configured to work with our main URL.

3. As we discussed in our teamwork plan, we decided to postpone some of our bells and whistles in our MVP. In the MVP, we don't take profile information into account when generating Chops (i.e., we don't look at movies in common): Chops are generated randomly, and so are movie suggestions. Users are able to enter movie titles, but our tagging system will be more advanced in our final project. We haven't yet implemented User ratings, either. Finally, we will clean up our UI a bit for our final project and thoroughly test our application to find security flaws.

4. To use AndChill, follow (2) and then create an account. After you create an account, navigate to your Chops page (there's a link in the top bar) to accept chops and the accepted Chops page to converse with your matches. Note that you will need to make more than one account in order to test the matching locally.
