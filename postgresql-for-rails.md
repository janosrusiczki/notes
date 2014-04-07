PostgreSQL for Ruby on Rails / Ubuntu 12.04
=====

## Setup

* `sudo apt-get install postgresql libpq-dev`
* `sudo -u postgres psql postgres`
* `\password postgres`
* `sudo -u postgres createdb mydatabase`

## Create, download & import a Heroku dump

* `heroku pgbackups:capture --expire --app myappname` - creates a backup
* `heroku pgbackups:url --app myappname` - displays the download link
* `pg_restore --verbose --clean --no-acl --no-owner -h localhost -U postgres -d mydatabase b257.dump`

## Links

* https://help.ubuntu.com/community/PostgreSQL
* http://www.amberbit.com/blog/2014/2/4/postgresql-awesomeness-for-rails-developers/
