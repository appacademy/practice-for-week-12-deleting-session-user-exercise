# Exercise: Deleting the Current User Session

In this exercise, you will learn how the current user session in a full-stack
application is stored on the frontend.

## Instructions

The current user session is the data about which user is currently logged in
and is performing user actions. This information is saved in the browser's data 
for the application. To remove the current user session and force the browser
to log you out of the application, you can remove the data that the browser
has stored for the application.

You will be observing this behavior in App Academy Open first, then another
application of your choice. You can replicate this forced log out on most web
applications.

Open a new tab and navigate to App Academy Open.

In the new tab, open up the Chrome Developer Tools to the "Application" tab.

There, you click on "Storage" in the side bar of that tab.

You should now see a button named "Clear site data" which will delete all the
frontend data that your browser has stored for App Academy Open. (Don't worry!
This will not delete your actual user data stored in the database. You will not
lose your App Academy Open progress, user information, or your classes.)

Refresh the tab. You should see the log in page of App Academy Open. App Academy
Open should now no longer recognize your user session until you log back in.

![clear-frontend-data]

Navigate to any application like [GitHub] that you have a user profile in. Make
sure you are logged in and then try to clear the site data like you did just now
for App Academy Open. If you refresh after doing so, you should no longer be
logged in.

This is because, whenever your browser makes a request to the server, it will
include your user session information in the request. The server will use that
information to identify which user is logged into the browser at the time that
the request is made.

[clear-frontend-data]: https://appacademy-open-assets.s3.us-west-1.amazonaws.com/Modular-Curriculum/content/week-12/clear-frontend-data-logout.gif
[GitHub]: https://github.com