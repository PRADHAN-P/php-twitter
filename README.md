Integrating With Twitter API In CodeIgniter

I needed to integrate Twitter API in one  of my web applications which uses CodeIgniter framework.

 
As their is no direct library available in CI for twitter integration, at first go this might look very difficult, but it is really simple.

 
Here is how you can do it..

First download the  Twitter class for PHP.
Put the class.twitter.php file in application/libraries folder.
Rename class.twitter.php to twitter.php ( to make it compatible with CI naming conventions).
Open twitter.php file and set following variables
var $username=’'; //twitter username
var $password=''; // twitter password
var $user_agent=''; //an identifier for twitter preferably email address

If you have followed these steps your integration is almost complete, now all you need to do is use the twitter library, here is an example to get you started :)

 $this->load->library('Twitter');
 $msg=’Just Integrated Twitter with CodeIgniter ’;
 $this->twitter->update($msg);
