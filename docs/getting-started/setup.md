# Setup

The installation of LinkStack is tailored to be as easy and user-friendly as possible.

In most cases, you will just be able to drop the LinkStack installation folder onto your web server, then visit this page with a browser to follow the setup wizard.

## 1. Download and unzip the latest release of the file

**for windows**, 
you can use this direct link to the [latest release](https://github.com/linkstackorg/linkstack/releases/latest/download/linkstack.zip) . unzip the files to your virtual host document root (or any other folder you prefer)
or if you need - check the previous releases from the [releases page on github](https://github.com/LinkStackOrg/LinkStack/releases)

**for linux**, 
download the files  
`wget https://github.com/linkstackorg/linkstack/releases/latest/download/linkstack.zip`

then unzip the downloaded file
`unzip linkstack.zip`
this will create a `\linkstack\` folder where you unzip the file. Move or copy the folder (contents) to your virtual host root.
to let laravel write logs and manage files, change folder owners to `www-data:www-data` or change folder rights accordingly [details](https://github.com/orgs/LinkStackOrg/discussions/510)

to prevent QueryException, make sure you have `php-sqlite3` installed.
go to your web browser and type in the address where linkstack files (index.php file, to be precise) is located.

the setup wizard will appear.

It will:

1. Check the server dependencies
2. Setup the database
3. Create the admin user
4. Configure the app

Setup wizard sometimes displays a few error messages as in [details](https://github.com/orgs/LinkStackOrg/discussions/510)
in case you see a blank setup page; visit `/skip` - this generates a default admin profile, and you can use the app like normal.[details](https://github.com/orgs/LinkStackOrg/discussions/383#discussioncomment-5476184)

after the installation, to go to the admin panel, you can go to example.com/home or example.com/dashboard - see [details](https://github.com/orgs/LinkStackOrg/discussions/450#discussioncomment-5997483)

**To ensure everything works as expected, please read the [installation requirements](./requirements.md).**
