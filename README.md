# Overview

shgrate is a simple database schema migration script for MySQL written in Bash.
It can be used as general purpose schema migration utility for a project. Let
say you're building an application using a framework but this framework does
not provide you the schema migration - then you can use shgrate to 'version
control' your database.

Most of the migration tools save the migrated actions into the database itself.
shgrate takes difference approach where all the migrated script is saved in
a directory so all the migrated script can be easily viewed without having
to connect to the database.

# Author

shgrate is written by Rio Astamal <me@rioastamal.net>

# License

shgrate is open source licensed under [MIT license](http://opensource.org/licenses/MIT).