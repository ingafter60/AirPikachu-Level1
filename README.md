# BUILDING LINKE AIRBNB APP 'AIRPIKACHU' LEVEL 1 USING Rails version: 6.0.3.4 & Ruby version: ruby 2.6.6p146

https://github.com/ingafter60/AirPikachu-Level1

## Task 1: Let's party

Install SQLiteBrowser1:21  
Install Atom2:57  
Install Ruby, Rails for MAC OS X 10.9 or higher  
Install Ruby, Rails for MAC OS X 10.6, 10.7 or 10.8  
Installing Ruby, Rails for Windows

### 1.1.1 Create a simple Rails Project with MySQL DB

    > rails new AirPikachu -d mysql --skip-webpack-install
    > cd AirPikachu
    > rails db:create
    > rails s
    > error
    > rails webpack:install
    > rails s
    > :)

        new file:   README.md

### 1.2.2 Install Bootstrap4

        modified:   Gemfile
        modified:   Gemfile.lock
        modified:   README.md
        deleted:    app/assets/stylesheets/application.css
        new file:   app/assets/stylesheets/application.scss
        modified:   app/javascript/packs/application.js

### 1.3.3 Create a new github repository

    > https://github.com/ingafter60/AirPikachu-Level1
        modified:   README.mdTask

## Taks 2: Basic project

### 06. What we're going to build in this task

    # Introduction of Taks 2
    > User registration
    > User login/logout
    > User update
    > User profile
    > Responsive navbar
    > Display logged in user

### 07. Create basic authentication

	> gem 'devise', '~> 4.6', '>= 4.6.2'
	> rails generate devise:install (bundle update is needed)
	> rails generate devise User
	> rails db:migrate
	mysql> DESC users;
	+------------------------+--------------+------+-----+---------+----------------+
	| Field                  | Type         | Null | Key | Default | Extra          |
	+------------------------+--------------+------+-----+---------+----------------+
	| id                     | bigint(20)   | NO   | PRI | NULL    | auto_increment |
	| email                  | varchar(255) | NO   | UNI |         |                |
	| encrypted_password     | varchar(255) | NO   |     |         |                |
	| reset_password_token   | varchar(255) | YES  | UNI | NULL    |                |
	| reset_password_sent_at | datetime     | YES  |     | NULL    |                |
	| remember_created_at    | datetime     | YES  |     | NULL    |                |
	| created_at             | datetime(6)  | NO   |     | NULL    |                |
	| updated_at             | datetime(6)  | NO   |     | NULL    |                |
	+------------------------+--------------+------+-----+---------+----------------+
	8 rows in set (0.00 sec)
	> rails g devise:views
	> rails s
	> http://localhost:3000/users/sign_up
	> sign up
	> rails s
	> :)
        modified:   Gemfile
        modified:   Gemfile.lock
        modified:   README.md
        new file:   app/models/user.rb
        new file:   app/views/devise/confirmations/new.html.erb
        new file:   app/views/devise/mailer/confirmation_instructions.html.erb
        new file:   app/views/devise/mailer/email_changed.html.erb
        new file:   app/views/devise/mailer/password_change.html.erb
        new file:   app/views/devise/mailer/reset_password_instructions.html.erb
        new file:   app/views/devise/mailer/unlock_instructions.html.erb
        new file:   app/views/devise/passwords/edit.html.erb
        new file:   app/views/devise/passwords/new.html.erb
        new file:   app/views/devise/registrations/edit.html.erb
        new file:   app/views/devise/registrations/new.html.erb
        new file:   app/views/devise/sessions/new.html.erb
        new file:   app/views/devise/shared/_error_messages.html.erb
        new file:   app/views/devise/shared/_links.html.erb
        new file:   app/views/devise/unlocks/new.html.erb
        modified:   app/views/layouts/application.html.erb
        modified:   config/environments/development.rb
        new file:   config/initializers/devise.rb
        new file:   config/locales/devise.en.yml
        modified:   config/routes.rb
        new file:   db/migrate/20201107040120_devise_create_users.rb
        new file:   db/schema.rb
        new file:   latest_specs.4.8
        new file:   latest_specs.4.8.gz
        new file:   prerelease_specs.4.8
        new file:   prerelease_specs.4.8.gz
        new file:   specs.4.8
        new file:   specs.4.8.gz
        new file:   test/fixtures/users.yml
        new file:   test/models/user_test.rb



	
Building navbar with partial view11:00  
Authentication with full name5:37  
Update authentication views17:04

Task 3: Gravatar, notification & transaction emails

What we're going to build in this task0:29  
Gravatar7:08  
Notification10:38  
Sending transactional email with Gmail10:40  
Sending transactional email with Mailgun6:58

Task 4: Facebook authentication

What we're going to build in this task0:51  
Create Facebook app1:33  
Create social authentication16:57  
Styling our views10:07  
Create user profile page8:59  
Create Edit Profile page

Task 4: Facebook authentication

16. What we're going to build in this task 00:00:51

17. Create Facebook app 00:01:34

18. Create social authentication 00:16:58

19. Styling our views 00:10:08

20. Create user profile page 00:09:00

21. Create Edit Profile page 00:12:39

Task 5: Creating Rooms

22. What we're going to build in this task 00:00:50

23. Create Room Model 00:06:02

24. Create Room Controller 00:15:42

25. Create Room View 00:22:46

26. Styling our views 00:09:19

27. Understanding the workflow 00:08:50

Task 6: Photos

28. What we're going to build in this task 00:00:55

29. Install Paperclip 00:02:27

30. Create Photo Model 00:04:47

31. Create Photo Controller 00:07:02

32. Create Photo View 00:10:35

33. Remove Photos with AJAX 00:08:36

34. Amazon S3 00:07:21

Task 7: Improving Room Creating Process

35. What we're going to build in this task 00:00:48

36. Add "Check" to Room Creating 00:09:43

37. Update the Photo Removing with AJAX 00:06:58

38. Issue with hidden fields 00:05:47

Task 8: Creating Views for Room

39. What we're going to build in this task 00:01:03

40. Create Room Index Page 00:08:52

41. Create Room Show Page 00:20:27

42. Add Google Map 00:11:03

43. Add Near-by Rooms 00:07:57

Task 9: Reservations

44. What we're going to build in this task 00:00:55

45. Create Reservations Model 00:04:07

46. Create Reservations View 00:06:12

47. Create Reservations Controller 00:09:19

48. Add jQuery Date Picker 00:05:38

Task 10: AJAX

49. What we're going to build in this task 00:00:57

50. Refactoring Reservation Form 00:08:53

51. AJAX for Start Date 00:19:51

52. AJAX for End Date 00:15:03

Task 11: More about Reservations

53. Create Your Trips Page 00:07:48

54. Create Your Reservations Page 00:13:26

55. Modify User Profile Page 00:06:39

Task 12: Creating Reviews

56. What we're going to build in this task 00:01:00

57. Creating Reviews Model 00:09:25

58. Creating Reviews Controller 00:17:47

59. Creating Reviews View 00:15:30

60. Creating Show Reviews Page 00:16:50

61. Adding jQuery Raty 00:02:33

62. Add Stars to Reviews 00:08:34

Task 13: Searching

63. What we're going to build in this task 00:01:06

64. Update Home Page 00:08:06

65. Creating Search Page 00:13:18

66. Create Search Function 00:17:12

67. Add Google Map 00:16:04

68. AJAX Searching 00:10:32

69. Add jQuery Pricing Slider 00:06:50

Task 14: Home Page

70. What we're going to build in this task 00:00:45

71. Modify Home Page 00:07:02

72. Improving Home Page 00:06:56

73. Auto Location Suggestion 00:07:12

What's Next? - Airbnb Level 2

74. About Level 2 - AirKong Project
