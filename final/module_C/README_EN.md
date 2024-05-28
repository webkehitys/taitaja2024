# Module C - Implementing an intranet for the site

**Competition time for the task: 3 hours**

This module will implement an intranet/administrative tool, utilising a database on a previously created site. The primary purpose of the intranet is to manage Hall of Fame games, their participants, and results. All data must come from the database, and you must create all the necessary database tables. You must establish a secure and protected database connection, including encryption using, for example, the Argon2 algorithm.

The code must be of high quality and maintainable for further development. It should be concise and simple and use techniques that make it easy to read, parse, and understand. Ensure you add clear instructions for using the intranet in the readme file.

Please note that this module is done simultaneously with the following module, and its results must be delivered at the end of the competition day.

- The intranet is available at `/admin`.
- Login is available at `/login`.

## Login

Access to the intranet site is only possible by logging in through the login page. If someone navigates to the intranet URL without logging in, they will be redirected to the login page. Once logged in, the username and logout button will appear in the main menu. The login form details must be validated before the form is submitted.

The following credentials should be used for login:

- **admin** with the password **taitaja2024** – admin role
- **user** with the password **taitaja2024** – user read/write access

## Intranet

The administrator can see all registered users on the intranet and add, edit, and delete users. Additionally, administrators can view all Hall of Fame games and events and add and edit games/events. Users can see their own profiles and the games they have permission to modify.

## User Roles

- admin (_superuser_)
- user with write/read permissions (_user_)

**Admin Can:**

- Log in and out
- Add new users
  - the default password for a new user is 'taitaja2024.'
- edit user passwords
- delete users
- add new games/events
  - required information when creating a new game includes title (mandatory), image (optional), default timestamp at the time of creation for the date, and the number of results displayed on the Hall of Fame page
- edit the game title, image, date, and the number of results shown
- add users to each game who have the rights to add and edit game results

**User Can:**

- log in and out
- edit their password
- Add and edit participants, results, and the number of results displayed on the game's/event's Hall of Fame page per game.
