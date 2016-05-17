### Overview

We have set up a PostgreSQL database on the Microsoft Azure cloud with support from the [Azure for Research](http://research.microsoft.com/en-us/projects/azure/default.aspx) program. Here we provide information on how to connect to this cloud database and gain experience querying and building your own tables.

#### Database architecture:

* PostgreSQL 9.4 with PostGIS extension on a Lunux Ubuntu Virtual Machine.

#### Connecting to the database

When a database gets built, the database manager sets controls on who can access the server. When deploying databases to the cloud it is especially important to pay attention to these security issues to ensure you do not lose data. We'll adopt the method of [ssh tunneling](http://www.postgresql.org/docs/9.1/static/ssh-tunnels.html) to give geoHack students access to our database. There are different methods depending on your operating system:

##### Windows Users:

1. Request a username and password from Anthony. This will be the same user/pw pair associated with your Linux login as well as your login to the PostgreSQL database.
2. Download and install putty from www.putty.org.
3. Open putty and create a new session. Type 40.118.160.139 in the "`host name"' section. Then give the session a name (here I’ve used “uwescience”) and type that under the “saved sessions” entry. Then click the “save” button.
4. Next we need to set the SSH Tunneling parameters. On the left, click on SSH/Tunnels. Then type “5432” in “show port” box, and “localhost:5432” in “destination” box:
5. IMPORTANT: after this, click on “sessions/logging” at the left (i.e. the starting screen again) and be sure to click “SAVE” one more time. Otherwise, the changes you just made to the tunneling parameters will not be saved with this session.
6. To start the session, click on “open”. Login with your user and password credentials. 

