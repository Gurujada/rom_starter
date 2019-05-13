# README

# Introduction
This is a brand new Rails 6.0.0.rc1 starter for developing Web Applications. The Application uses [ROM-RB](https://rom-rb.org) as the ORM layer.

Here are the basic changes that are done from the standard "rails new"

* The application is created with `rails new --skip-active-record --webpack --skip-sprockets --skip-test`
* The gems `pg`, `rom-rails`, `rom-sql` are added
* I prefer using `rspec-rails` for testing. The gem is added and installed.
* An initializer is added in `config/rom.rb` according to [Getting Started - Rails Setup](https://rom-rb.org/5.0/learn/getting-started/rails-setup/index.html)
* The gem `dotenv-rails` is added. The database configuration is added in the file .env.development
* The test database configuration is added in the file .env.test
* Added a line `rom/sql/rake_task`. This line will enable rake tasks for generating and running migrations from `rom-sql`
# How to Use

* Clone the repo
* Change database configurations including username and password in `.env.development` and `.env.test` 
* In `application.rb` change the  module name from `RomStarter` to your application name
# License
MIT License. Feel free to use the work if it is useful in anyway for you.
# Goal
Make an enterprise-ready application skeleton to give a headstart for developers in Enterprise Application Development. 
I thank [@radar](https://github.com/radar) for the inspiration. 