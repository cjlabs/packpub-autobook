# packpub-autobook
auto booking for free e-book from packpub


- change to codeception directory
- composer install
- copy file tests/acceptance/ClaimCept.php.dist and change the filename to ClaimCept.php
- edit file ClaimCept.php, change the email and password with your packpub creadential 
- testing with php using : php codeception/vendor/bin/codecept run acceptance ClaimCept
- added cronjob to makes this automatically

0 11 * * * /usr/local/bin/php  /yourpath/packpub-autobook/codeception/vendor/bin/codecept run acceptance ClaimCept


