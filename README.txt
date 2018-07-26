This is the source code for the article Create a PHP OAuth Server by
Jamie Munro available at http://sitepoint.com/creating-a-php-oauth-server

OAUTH-PHP Library

How it work:
1. Copied code from article.
2. Downloaded "oauth-php" from GitHub and copied it to vendor (folders and files)
3. Go to folder Include/common.php -> and configure DB connection. This file is included in every php file and it uses autoload to incude all 'oauth-php' library to commom.php
4. Go to folder sql/schema.sql and import it to phpMyAdmin. It contains 1 single users database.
5. Go to vendor/store/mysql/mysql.sql and import it to phpMyAdmin.  It contains 1 single users database 6 tables(oauth_server_registry, oauth_server_token, oauth_server_nonce, oauth_log, oauth_consumer_token, oauth_consumer_registry).

Test:
1.Go to public/register.php, it will dispaly registation form, the data from this form will be saved  to SQL => oauth(DB name)-> oauth_server_registry(saves Consumer key, Consumer secret, callback URI, etc)
 and to table {users} (name, email, date.)



MB:
public/access_token.php, login.php must be reached with ajax ???


//Example 
Save these values!

Consumer key: ca18302e26ce2bf95c17ec0defe027fa05b59be7e

Consumer secret: 1db135758abbec7b8c2a446542dd4898