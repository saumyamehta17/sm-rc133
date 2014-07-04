Railscast sm-rc133
===================
capistrano
````
It is ruby program that is set of tools to deploy your application to server
```
Gemfile
```
gem 'capistrano' , group: :development
bundle install
```
run command capify . Or cap install depending on version
```
run this command which will create a capfile for deployment receipe at config/deploy.rb
```
creating task and callbacks in deploy.rb
```
see deploy.rb
Task run --  cap hello
Using callback -- after
```
setting value
```
set :name, 'value'
to use default vaue use fetch else simply by string interpolation
```

Now tell capistrano to invoke stage
```
Rake::Task[:production].invoke in capfile at last
And then run cap . commands
```
Four type of server are there
```
cloud server, Virtual private server, dedicated server, shared server
```
Server setup
```
Ways:
Heroku
VPS - like DigitalOcean , linode or webinar - it will provide a blank server and fill accordingly,
   a) webserver - ngnix or apache
   b) unicorn or phusion passenger- http server for rails application
   c) database - postgres or mysql
   d) ruby manager - rbenv or rvm
   c) ubuntu
```
Using DigitalOcean
```
create a droplet there, you will have ssh root@ip and root password
run at terminal
Now install your settings as:
 a) apt-get update


335, 133, 337 railscast
```