FROM mysql:5.5
MAINTAINER Quintessence

ADD files/run_db files/init_db schema/Chinook_MySql.sql /tmp/

# run_db will start the MySQL daemon and will seed
# the database if /var/lib/mysql is empty
RUN /tmp/init_db
ENTRYPOINT "/tmp/run_db"
