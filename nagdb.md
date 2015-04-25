# Introduction #

nagdb is a tool which is designed to easily enable you to keep your Nagios status in a database.  Why might you want to do that?  Easy to query, easy to script up otherwise impossible actions (e.g. acknowledge all of the services for a given host).  As delivered, the script uses the python-mysql (MySQLdb) module for database access.  Changing that is fairly trivial.


# Installation #

  1. Copy the file somewhere on your Nagios server.  Personally, I recommend ~nagios/libexec.
  1. Create a schema for nagdb to use.
  1. Update nagdb with the database connection information
  1. Run the script as a user who can access ~nagios/var/nagios.log
  1. Watch the database fill with data!