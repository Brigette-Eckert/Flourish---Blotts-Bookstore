
#About

Flourish and Blots fake bookstore built with Drupal 7 as part of self study following Epicodus curriculum.

# Instructions:

1. Download Drupal version 7.51

2. Replace the sites folder with the enclosed sites folder

3. Import the Database Dump

  a. Open phpMyAdmin and click on the "Import" tab.

  b. Leave all the default settings and make sure the character set is "utf-8"

  c. Now click on the "Choose File" button next to "Browse your computer" and select the .sql.zip file we included in our sites/db-backup folder. It's okay to leave it zipped.

  d. Then click the "Go" button on the bottom left.

4. Create the Database User (not needed if using Acquia Dev Desktop)

  a. Lastly, we must recreate the database username/password that Drupal uses to store things in the database. We do this the same way we did when we created the database.

  b. After importing the .sql.zip file, select the "Privileges" tab and click on "Add User".

  c. Use the same username and password from before. (If we have forgotten what that was, we can always find that information in settings.php, or in the PDO Exception error message we saw displayed in the browser.)

  d. After importing the database, if you have any trouble logging in with your Site Maintenance account, clear your browser's cookies by clearing the browser history.


#Project Instructions
*Create 2 basic pages - an "About" page, and a "Locations" page.

*Enable and configure the Contact module. Include a Contact form with a "Contact" link in the main menu. Make sure that anyone, regardless of their user role, can use the form to send you website feedback.

*Install the Views module, the Features module and the Strongarm module, and all their dependencies.

* Create a feature called "Site Configuration". Make the feature track the strongarm variables site_name, site_slogan, theme_default and site_frontpage (The URL for the page displayed as your frontpage). Generate the feature in your modules directory, then enable it in the Features management page and then commit the feature with your repository.
Then change the site's default theme, name and slogan and configure the website so that that the "About" page is the front page

* Create a "Book Review" custom content type. The title field should be labelled "Book Title". It should also include fields for "Book Author", "Rating", and "Review Body".
  The "Book Title", "Book Author", "Rating", and "Review Body" fields should be required.
  The rating should be chosen with either a menu or radio buttons.
  The fields should be in the order "Book Title", "Book Author", "Rating", then "Review Body" when you fill out the form to add an instance of the book review content type.
  Create a feature called "Book Review" for your new content type and then generate it in your modules directory

*Create a view for the Book Review content type called "New Books". Don't bother creating a page for it, just create a block for it. The block should display the 3 newest book reviews as an unformatted list of linked titles, so that users can click on the title of a new book to go read the review of it. Don't use a pager.
  Name the block and display it in an easily visible region. Add at least 4 book reviews to verify that it is working.
  Add the "New Books" view to your "Book Review" feature and then recreate it, generating the files in your modules directory as usual.

*Create a custom "Reviewer" role.
  * The Reviewer role should have all the same permissions as an authenticated user, and also be able to create new book reviews.
  *They should be able to edit and delete their own book reviews, but not anyone else's
  *Create an account for a user who is a Reviewer to test it out.

*Create a special coupon to display as a block on the front page which is visible to authenticated users and not anonymous users. It should say something like "This week: use this coupon code to get 25% off on all Science Fiction!"
*No need to worry about shopping cart functionality.


#To Do
 Use taxonomy on views to fliter by term -change settings in views
