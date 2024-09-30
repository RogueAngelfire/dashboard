<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

You may also try the [Laravel Bootcamp](https://bootcamp.laravel.com), where you will be guided through building a modern Laravel application from scratch.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains thousands of video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the [Laravel Partners program](https://partners.laravel.com).

### Premium Partners

- **[Vehikl](https://vehikl.com/)**
- **[Tighten Co.](https://tighten.co)**
- **[WebReinvent](https://webreinvent.com/)**
- **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
- **[64 Robots](https://64robots.com)**
- **[Curotec](https://www.curotec.com/services/technologies/laravel/)**
- **[Cyber-Duck](https://cyber-duck.co.uk)**
- **[DevSquad](https://devsquad.com/hire-laravel-developers)**
- **[Jump24](https://jump24.co.uk)**
- **[Redberry](https://redberry.international/laravel/)**
- **[Active Logic](https://activelogic.com)**
- **[byte5](https://byte5.de)**
- **[OP.GG](https://op.gg)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).


## Laravel Framework Assignment

## by Robin Collins

## Project Purpose

## Step to install Laravel

1, Install XAMPP (or another .....)
2, Install Composer
3, Set up system variables (Windows)
4, Download Varavel
5, Create new Laravel project
6, Set up database

## Set up for Windows

Open up the Command prompt. Type cmd in the search bar.

Go to https://apachefriends.org

# XAMPP instalation

If you already have XAMPP make sure the latest version is installed.

# Composer instalation

https://getcomposer.org

Click download the latest version

    install for all users.

    click next (make sure developer mode is unchecked).

    Make sure the path is where PHP is installed normally C:\xampp\php\php.exe
    
    Click Next.
    
    Then Next again make sure boxes still unchecked.
    
    Now click install.

    Notifications will appear here suggesting a reboot maybe required.

    Click Next again.

    Then click finish (unchecking any boxes).

Click this PC

Go into properties

Then system settings

Then Advanced System Settings - This will open a small window.

Click on the option of enviromental variables.

In the bottom section it will say system variables.
Click New.

From C:\xampp\php copy the path and paste this into the variable value section make sure you add a backslash(\) and php.exe to the path so it looks like this C:\xampp\php\php.exe

In the varaible name section add the variable name PHP

Then click OK

Now to set composer as variable

Goto this PC

Local Disk

ProgramData (This is a hidden file so click view and click the check box to reveal hidden items).

Then click ComposerSetup

Click bin

then copy the path C:\ProgramData\ComposerSetup\bin

Create a new system variable

Add the Variable Name Composer

the paste the variable value C:\ProgramData\ComposerSetup\bin

click OK

To check Composer is now in the System.

Close and restart the command prompt

Then type

composer --version

The composer and PHP versions should be displayed. Therefore, confirms everything has installled correctly.

NOTE: If this doesn't work try restarting the computer.

# Install Laravel

Still in the command prompt type the following:

composer global require laravel/installer

this will start installing Laravel

# Connection Laravel with XAMPP

Go into This PC > Local Disk > xampp > php

Scroll down until you find the file php.ini

Open this in the text editor (VS code).

Click control F (command f on Mac) which will open the search.

Then search for extension=zip

Make sure this is uncommented by removing the semi colon.

next remove the ; from:

extension=fileinfo 

Normally found at line 930

Do the same on line 938

extension=mysqli 

NOTE: Lines and commented out lines can vary

Make sure the comment remains on line 942

;extension=openssl

Now you can close this file.

Open a new terminal within VS Code (at this stage cmd prompt terminal not required).

Make sure the correct file is open from xampp

Opening program folder click xampp htdocs then dashboard (open or drag and drop into VS Code).

Open the new terminal

You wil see that the termainal path is correct 

c:\xammpp\htdocs\dashboard 

type into the terminal:

laravel new laravel

(The second laravel is the project name so it could be laravel-app or myfirstlaravel anything you want without breaks in the text and exotic sybols).

NOTE: An error message will appear!

Restart VS Code

Make sure you go back into the correct folder dashboard

In the terminal using the up keys scrol for the previous command or add it again:

laravel new laravel 

click enter and it will run the intilation:

You will be given options at this stage:

Would you like to install a starter kit?

I chose to write none

Which testing framework do you prefer?

I chose option 0 pest as more modern.

Which database will your application use?

NOTE: At this stage I open my XAMPP control pannel and start the Apache and mySQL servers.

Go back or open web browser

type:

localhost/phpmyadmin

when phpMyAdmin is open:

Click on Databases

Name it laravel (Name it after name of your project).

Then click Create

Once done you see the database appear on the side of the screen.

If click there is nothing going on within it.

Quicky switch back to VS Code

type:

mysql

ckick enter

Defalt database updatedd. Would you like to run the default database migrations?

write:

yes

This will set up the tables

Now go back to the browser for PhpMyadmin and click the refresh button and the table will now appear.

Laravel is now set up.

## Set up for Mac OS

Open up the terminal or iTerm if installed on the search bar (I prefer mine pinned to the bar).

Go to https://apachefriends.org

# XAMPP instalation

If you already have XAMPP make sure the latest version is installed.

# Composer instalation

https://getcomposer.org

Composer is slightly different on a mac than windows.

start by going into the user local bin drive to set up Composer Globally.

cd /usr/local/bin 

if this directory doesn't exsit then type the following.

sudo mkdir -p /usr/local/bin

Now download the Composer installer

sudo curl -sS https://getcomposer.org.installer | sudo php

Composer is now installed under the name of composer.phar

Therefore to refrain from having to type the extension in every time it will need renaming.

mv composer.phar composer

now type composer in the terminal:

composer

The intructions will appear.



## After Laravel install

Type in local host on the browser.
