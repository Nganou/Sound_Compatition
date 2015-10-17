sound_competition
=============

Common code for the Relational Databases and Full Stack Fundamentals courses

tournament.sql:

Creates the tables for the tournament and consists of:
	- Tournament database: Consists of the Match(battle) organizer's Informations
	- Matches database: consists of matches(battles), winner and loser.
	- Players database: consists of an artist id, name, song(instrumental) entered in the contest, location
	- Results database: Consists of the result of a match(battle), the winner, status of match in win/lose/draw

tournament.py


Install Vagrant and VirtualBox
Clone the wave_comp repository
Launch the Vagrant VM

=======================
 Run the Application
=======================

1. vagrant up <br>
If you are getting the following error, try changing the vagrant operating system to ubuntu 64 bit:
default: SSH address: 127.0.0.1:2222
default: SSH username: vagrant
default: SSH auth method: private key
default: Warning: Connection timeout. Retrying...
default: Warning: Remote connection disconnect. Retrying...
default: Warning: Remote connection disconnect. Retrying...

2. vagrant ssh
3. cd /vagrant/tournament
4. Create the database: psql \i tournament.sql
5. Exit out of psql: \q
6. Run the application: ./tournament_test.py
