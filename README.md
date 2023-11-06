### [Basic writing and formatting syntax for MD Fille](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
# Developer Manual

# Table Of Contents

1. [PC Setup](#pc-setup)
2. [Git Set Up](#github-set-up)
3. [WordPress Coding Standard](#wordpress-coding-standered)
4. [WordPress Plugin Development](#wordpress-plugin-development)
5. [WordPress Theme Development](#wordpress-theme-development)
6. [WordPress Rest API Development](#wordpress-theme-development)
7. [Unit Testing](#wordpress-theme-development)
8. [React Tutorials](#react-tutorials)
9. [GrumPHP](#grumphp)

# PC Setup
1. IDE will be PHPStorm
   1.  Import IDE Settings. Please visit the below link to import IDE settings.
   2. [How to import IDE Settings](https://www.jetbrains.com/help/phpstorm/sharing-your-ide-settings.html#import-export-settings)
2. [Node.js LTS version](https://nodejs.org/en/download), [XAMPP](https://www.apachefriends.org/download.html) or [MAMP](https://www.mamp.info/en/downloads/), [Git](https://git-scm.com/downloads)
3. If you're using MacOs then install [brew](https://brew.sh/)
4. Create an account to [atlassian](https://www.atlassian.com/) for task management by JIRA software.
5. Connect with official [slack](https://slack.com/) channel for communication with team.


# GIT Setup
### [ GIT Installation](https://git-scm.com/downloads)
Then connect your git account with the current PC through `SSH Key`. Read this article to connect with your PC.

[Adding a new SSH key to your GitHub account](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account).


### How to manage multiple GitHub accounts on a single machine with SSH keys

https://www.freecodecamp.org/news/manage-multiple-github-accounts-the-ssh-way-2dadc30ccaca/
```
FOR SWITCHING ACCOUNT
Delete current ssk key 
ssh-add -D
setup new ssh key
ssh-add ~/.ssh/id_azizulhasan

Change username and email
Git config user.name “username”
Git config user.email “example@gmail.com”
```


### GitFlow Setup
Gitflow is an alternative Git branching model that involves the use of feature branches and multiple primary branches.
   1. [GitFlow Installation](https://github.com/petervanderdoes/gitflow-avh/wiki/Installation)
   2. [GitFlow Cheat Sheet](https://danielkummer.github.io/git-flow-cheatsheet/)

# WordPress Coding Standard

[WordPress Coding Standards ](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/) **by WordPress must read documentation for coding standard.**
### Why have coding standards?
Coding standards help avoid common coding errors, improve the readability of code, and simplify modification. They ensure that files within the project appear as if they were created by a single person.

Following the standards means anyone will be able to understand a section of code and modify it, if needed, without regard to when it was written or by whom.

If you are planning to contribute to WordPress core, you need to familiarize yourself with these standards, as any code you submit will need to comply with them.

### Language-specific Standards
1. CSS Coding Standards
2. HTML Coding Standards
3. JavaScript Coding Standards
4. PHP Coding Standards

[WordPress Coding Standards for PHP_CodeSniffer](https://github.com/WordPress/WordPress-Coding-Standards)


# WordPress Plugin Development
The best resource for learning about WordPress plugin development is [Introduction to Plugin Development](https://developer.wordpress.org/plugins/intro/) by WordPress.
**WebAppick** provides and prefer developers to learn about WordPress plugin development from a tutorial by **Hasin Hayder**. Here is the link
[ওয়ার্ডপ্রেস প্লাগইন ডেভেলপমেন্ট](https://learnwith.hasinhayder.com/wp/course/wordpress-plugin-development/).



**Credentials**: 
```
username: 
password:
```
If these credentials are not working please ask for credentials to who are concern.


## IMPORTANT TOPICS TO UNDERSTAND
1. **[Plugin Security](https://developer.wordpress.org/plugins/security/)**
   1. Check User Capability.
   2. Data Validation
   3. Data Sanitization
   4. Data Escaping
   5. Nonce
2. **[Hooks](https://developer.wordpress.org/plugins/hooks/)**
   1. Few Methods To Understand Hooks
   ```
   1. add_action()
   2. do_action()
   3. add_filter()
   4. apply_filter()
   5. has_filter()
   6. did_action()
   7. remove_filter()
   8. remove_action()
   9. current_action()
   10. current_filter()
   12. remove_all_actions()
   13. remove_all_filters()
   ```
3. **[AJAX](https://developer.wordpress.org/plugins/javascript/ajax/)**
4. **[Cron Job ](https://developer.wordpress.org/plugins/cron/)**
4. **[Internationalization](https://developer.wordpress.org/plugins/internationalization/)**
4. **[ShorCode](https://developer.wordpress.org/plugins/shortcodes/)**
4. **[Custom Post Type](https://developer.wordpress.org/plugins/post-types/)**
4. **[Taxonomies](https://developer.wordpress.org/plugins/taxonomies/)**


   
# WordPress Theme Development
The best resource for learning about WordPress theme development is [Introduction to Theme Development](https://developer.wordpress.org/themes/getting-started/) by WordPress.
**WebAppick** provides and prefer developers to learn about WordPress plugin development from a tutorial by **Hasin Hayder**. Here is the link
[ওয়ার্ডপ্রেস থিম ডেভেলপমেন্ট](https://learnwith.hasinhayder.com/wp/course/wordpress-theme-development/).

**Credentials**:
```
username: 
password:
```
If these credentials are not working please ask for credentials to who are concern.

# WordPress Rest API Development
The best resource for learning about WordPress Rest API development is [REST API Handbook ](https://developer.wordpress.org/rest-api/~) by WordPress.
**WebAppick** prefer developers to learn about WordPress Rest API development from a tutorial by **Tarek Hasan**. Here is the link
[Introduction to REST API in WordPress](https://www.youtube.com/watch?v=KoxcDK76zzI&t=14s&ab_channel=TareqHasan).

> [!WARNING]
> 
> This tutorial is not beginner friendly. First read and practice about Rest API from documentation by WordPress mentioned above.
> Then try to view this tutorial by **Tarek Hasan**

# Unit Testing With MACOS
### Project Setup
We'll configure codeception for wpunit testing. Below step by step shown how to set up project.
1. Add ```require-dev``` composer packages to `composer.json` file
   ``
   "codeatcode/codeatcs": "^1.0",
   "codeception/codeception": "^4.2",
   "codeception/module-asserts": "^1.0",
   "codeception/module-cli": "^1.0",
   "codeception/module-db": "^1.0",
   "codeception/module-filesystem": "^1.0",
   "codeception/module-phpbrowser": "^1.0",
   "codeception/module-rest": "^1.2",
   "codeception/module-webdriver": "^1.0",
   "codeception/util-universalframework": "^1.0",
   "dealerdirect/phpcodesniffer-composer-installer": "^0.7",
   "ergebnis/composer-normalize": "^2.6",
   "lucatume/function-mocker": "~1.0",
   "lucatume/wp-browser": "^3.1",
   "phpro/grumphp": "^1.13",
   "phpunit/phpunit": "^9.2",
   "szepeviktor/phpstan-wordpress": "^1.1.2",
   "php-webdriver/webdriver": "^1.12"
``
2. Set up the `codeception.dist.yml` file
3. Set up `.env` file. fill params of `env` file constants
   ``
   WP_ROOT=/Applications/MAMP/htdocs/ctxfeedpro
   WP_URL='http://localhost:8888/ctxfeedpro'
   WP_URL_S='http://localhost:8888/ctxfeedpro'
   WP_DOMAIN='localhost:8888/ctxfeedpro'
   DB_HOST='localhost'
   DB_NAME='wordpress64'
   TEST_DB_NAME='wordpress64'
   DB_USER='root'
   DB_PASSWORD='root'
   DISABLE_ESLINT_PLUGIN=true
   EXTEND_ESLINT=true
   ``
   4. PC Set up
      Required PHP version 7.4. MacOS usually uses ``homebrew`` PHP. We have to use ``MAMP Pro`` PHP for wpunit test.
      Here is the process to do it
      run the command in your terminal ```sudo nano ~/.bash_profile``` it will open your `bash_profile` file.
      Add the following to the file
```
export PATH="/Applications/MAMP/bin/php/php7.4.21/bin:$PATH"
export PATH=$PATH:/Applications/MAMP/Library/bin
```
 Here first line tels which php version will be used  during unit testing. Second tels the path of 
      ``MySQL`` 
      After the setting php and mysql to ``bash_profile`` now run command
      ```source ~/bash_profile```.
      Now all setup is done.
5. Start Unit Test
   Write test case and start testing by this command. 
```
php ./vendor/bin/codecept run tests/wpunit/Common/DropdropOptionTest.php —debug

```
   
### Resource to study
1. [How to override the path of PHP to use the MAMP path?](https://stackoverflow.com/questions/4145667/how-to-override-the-path-of-php-to-use-the-mamp-path)
2. [How to add MySQL to $PATH variable to resolve "mysql: command not found"?](https://apple.stackexchange.com/questions/176786/how-to-add-mysql-to-path-variable-to-resolve-mysql-command-not-found)


```
Make alias in Mac
alias codecept="php ./vendor/bin/codecept run"

PHPSTAN TEST
 php ./vendor/bin/phpstan analyse libs/webappick-product-feed-for-woocommerce/V5/Common/Helper.php

PHPCS TEST
php ./vendor/bin/phpcs libs/webappick-product-feed-for-woocommerce/V5/Common/Helper.php  

CODECEPT TEST
php ./vendor/bin/codecept run tests/wpunit/Common/DropdropOptionTest.php —debug

```

# React Tutorials
# GrumPHP
Sick and tired of defending code quality over and over again? GrumPHP will do it for you! This composer plugin will register some git hooks in your package repository. When somebody commits changes, GrumPHP will run some tests on the committed code. If the tests fail, you won't be able to commit your changes. This handy tool will not only improve your codebase, it will also teach your co-workers to write better code following the best practices you've determined as a team.

GrumPHP has a set of common tasks built-in. You will be able to use GrumPHP with a minimum of configuration.

[Installation & Documentation ](https://github.com/phpro/grumphp#installation)










