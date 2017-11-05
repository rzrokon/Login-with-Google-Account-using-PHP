# Login-with-Google-Account-using-PHP
Google oAuth API provides an easy and powerful way to integrate login system on the website. The web developers can implement login and registration system in the web application using Google OAuth 2.0. Google login system helps to increase subscribers on your website. Because nowadays almost all users have a Google account and they can log in with their Google account without registration on your website.

# Database Table Creation

To store the Google+ profile information, you need to create a database and a table. At first, create a database (like codexworld) and run the below SQL on the database. The following SQL creates a users table to the database for inserting the user profile information.

```sh

CREATE TABLE `users` (
 `id` int(11) NOT NULL AUTO_INCREMENT,
 `oauth_provider` varchar(255) COLLATE utf8_unicode_ci NOT NULL,
 `oauth_uid` varchar(255) COLLATE utf8_unicode_ci NOT NULL,
 `first_name` varchar(100) COLLATE utf8_unicode_ci NOT NULL,
 `last_name` varchar(100) COLLATE utf8_unicode_ci NOT NULL,
 `email` varchar(255) COLLATE utf8_unicode_ci NOT NULL,
 `gender` varchar(10) COLLATE utf8_unicode_ci NOT NULL,
 `locale` varchar(10) COLLATE utf8_unicode_ci NOT NULL,
 `picture` varchar(255) COLLATE utf8_unicode_ci NOT NULL,
 `link` varchar(255) COLLATE utf8_unicode_ci NOT NULL,
 `created` datetime NOT NULL,
 `modified` datetime NOT NULL,
 PRIMARY KEY (`id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8 COLLATE=utf8_unicode_ci;

```