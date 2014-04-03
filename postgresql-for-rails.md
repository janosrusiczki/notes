PostgreSQL for Ruby on Rails / Ubuntu 12.04
=====

## Setup

* `sudo apt-get install postgresql libpq-dev`
* `sudo -u postgres psql postgres`
* `\password postgres`
* `sudo -u postgres createdb mydatabase`

## Import a Heroku dump

`pg_restore --verbose --clean --no-acl --no-owner -h localhost -U postgres -d mydatabase b257.dump`

## Links

* https://help.ubuntu.com/community/PostgreSQL
* http://www.amberbit.com/blog/2014/2/4/postgresql-awesomeness-for-rails-developers/
