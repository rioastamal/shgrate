## Overview

shgrate is a simple database schema migration script for MySQL written in Bash.
It can be used as general purpose schema migration utility for a project. Let
say you're building an application using a framework but this framework does
not provide you the schema migration - then you can use shgrate to 'version
control' your database.

Most of the migration tools save the migrated actions into the database itself.
shgrate takes difference approach where all the migrated script is saved in
a directory so all the migrated script can be easily viewed without having
to connect to the database.

shgrate needs three directories in order to do its job. 

Directory | Use for
----------|--------
migrations | Used to store the SQL migration scripts
migrated | Used to store actions which has been migrated
rollback | Used to store the SQL rollback scripts

## Requirements

shgrate require Bash (tested with Bash 4.3.11), MySQL client binary and other shell core utilities:

* awk
* date
* diff
* grep
* logger
* sort
* tr

Those shell utilities should be available in most Linux distribution and Unix
compatible OS such as Mac OS X - even Windows using cygwin.

## Installation

Clone the project repository via github:

```
$ git clone github.com/astasoft/shgrate
```

Another altertive is download the zip tarball and extract it somewhere on your box.

shgrate needs 

## Author

shgrate is written by Rio Astamal <me@rioastamal.net>

## License

shgrate is open source licensed under [MIT license](http://opensource.org/licenses/MIT).
