Portable Apache + MySQL + PHP for Windows
=========================================

Note:  MySQL is pretty much a dead project.  They don't really fix bugs or security vulnerabilities.  The developers jumped ship and went to Maria DB or other projects.  See my newer [Portable Apache + Maria DB + PHP for Windows](https://github.com/cubiclesoft/portable-apache-maria-db-php-for-windows) GitHub repo.

This project is for web developers who prefer manually editing configuration files and want "manual" but quick startup of Apache and MySQL (no Windows services).  No more hunting for ZIP files for each separate piece of software.

If XAMPP and similar incarnations are not really your style (e.g. you prefer the command-line and think phpMyAdmin is for weaklings), then this project might be more up your alley.  Note that the primary purpose of this project is to set up a quick-and-dirty local WAMP install that just works and is not intended for use on production servers.

GitHub is a perfect fit for this sort of project.  The latest code resides here, so updating is a matter of running a 'git pull'.  Set up a Task Scheduler job to update this project automatically or use it as a submodule in your own Git project.  If you know of any changes that need to be made, submit a pull request so that everyone benefits.

Features
--------

* Classic Apache + MySQL + PHP combo in a portable format.
* A flashback from the past:  Batch files!  install.bat, start_server.bat, and stop_server.bat to install, start, and stop the software respectively.
* Installation is designed to just adapt paths to the current host.  No registry mess, no Windows services, no problem.
* Has a liberal open source license.  MIT or LGPL, your choice.  (Only applies to the new files that this project adds.  Each product has its own separate license.  See below.)
* Designed for relatively painless integration into your Windows environment.
* Sits on GitHub for all of that pull request and issue tracker goodness to easily submit changes and ideas respectively.

Useful Information
------------------

Do the whole 'git clone' thing to obtain the latest release.  Then run 'install.bat' to get the configuration files set up quickly.  Note that you will need approximately 2GB free to successfully complete the installation.

Run 'start_server.bat' to start the Apache web server and MySQL database server.  To stop both servers, run 'stop_server.bat'.

To upgrade to the latest version, stop the servers with 'stop_server.bat', run 'git pull', and then run 'upgrade.bat'.

Troubleshooting
---------------

Requires 'taskkill.exe' for 'stop_server.bat' to work properly.  This is part of Windows XP and later.

Sources
-------

The Apache web server is under the Apache License, Version 2.0.  (http://www.apache.org/licenses/LICENSE-2.0.html)

http://www.apachelounge.com/download/win32/

The MySQL database server is under the MySQL GPL EXCEPTIONS clause for FOSS.  (http://www.mysql.com/about/legal/licensing/foss-exception/)

http://dev.mysql.com/downloads/mysql/

The PHP scripting language is under the PHP License.  (http://www.php.net/license/3_01.txt)

http://windows.php.net/download/
