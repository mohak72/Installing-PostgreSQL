# Installing-PostgreSQL
Installing PostgreSQL on ubuntu
Step1 :-sudo apt-get install wget ca-certificates
        wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -
        
Step2 :-sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt/ `lsb_release -cs`-pgdg main" >> /etc/apt/sources.list.d/pgdg.list'

Step3 :- sudo apt-get update
         sudo apt-get install postgresql postgresql-contrib
  # Installing pgadmin4      
Step4 :- sudo apt-get install pgadmin4 pgadmin4-apache2

http://example.com/pgAdmin4


#Connect as postgres user and set admin password.

[root@postgresql-01 ~]# su - postgres
-bash-4.2$ psql
psql (11.4)
Type "help" for help.

postgres=# ALTER USER postgres WITH PASSWORD '123';
ALTER ROLE
postgres=# \q
-bash-4.2$ exit
logout
