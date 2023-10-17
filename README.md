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
3. If you're using macOS then install [brew](https://brew.sh/)
4. Create an account to [atlassian](https://www.atlassian.com/) for task management by JIRA software.
5. Connect with official [slack](https://slack.com/) channel for communication with team.


# GIT Setup
### [ GIT Installation](https://git-scm.com/downloads)
Then connect your git account with the current PC through `SSH Key`. Read this article to connect with your PC.

[Adding a new SSH key to your GitHub account](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account).

### GitFlow Setup
Gitflow is an alternative Git branching model that involves the use of feature branches and multiple primary branches.
   1. [GitFlow Installation](https://github.com/petervanderdoes/gitflow-avh/wiki/Installation)
   2. [GitFlow Cheat Sheet](https://danielkummer.github.io/git-flow-cheatsheet/)

# WordPress Coding Standard

[WordPress Coding Standards ](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/) **by WordPress must read documentation for coding standard.**
### Why have coding standards?
Coding standards help avoid common coding errors, improve the readability of code, and simplify modification. They ensure that files within the project appear as if they were created by a single person.

Following the standards means anyone will be able to understand a section of code and modify it, if needed, without regard to when it was written or by whom.

If you are planning to contribute to WordPress Core, you need to familiarize yourself with these standards, as any code you submit will need to comply with them.

### Language-specific Standards
1. CSS Coding Standards
2. HTML Coding Standards
3. JavaScript Coding Standards
4. PHP Coding Standards

[WordPress Coding Standards for PHP_CodeSniffer](https://github.com/WordPress/WordPress-Coding-Standards)


# WordPress Plugin Development
The best resource for learning about WordPress plugin development is [Introduction to Plugin Development](https://developer.wordpress.org/plugins/intro/) by WordPress.
**WebAppick** provides and prefers developers to learn about WordPress plugin development from a tutorial by **Hasin Hayder**. Here is the link
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

# Unit Testing
# React Tutorials
# GrumPHP
Sick and tired of defending code quality over and over again? GrumPHP will do it for you! This composer plugin will register some git hooks in your package repository. When somebody commits changes, GrumPHP will run some tests on the committed code. If the tests fail, you won't be able to commit your changes. This handy tool will not only improve your codebase, it will also teach your co-workers to write better code following the best practices you've determined as a team.

GrumPHP has a set of common tasks built-in. You will be able to use GrumPHP with a minimum of configuration.

[Installation & Documentation ](https://github.com/phpro/grumphp#installation)










