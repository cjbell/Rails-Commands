=Learning Rails Commands

Create new app
	
	rails new _name_ --skip-test-unit

Generating

	rails generate controller Foos --no-test-framework
	rails generate model Foo title:string

==Gems

Modify gem file 
	
	group :development, :test do
	  gem 'sqlite3', '1.3.5'
	  gem 'rspec-rails', '2.9.0'
	  gem 'annotate', '~> 2.4.1.beta'
	end

Update gems

	bundle install --without production

==RSpec

RSpec on install
	
	rails generate rspec:install

Run Tests

	bundle exec rspec spec/

==Rake / Database

	rake db:migrate
	rake db:rollback VERSION
	rake db:

==Misc

Annotate models

	gem 'annotate', '~> 2.4.1.beta'
	bundle exec annotate --position before

Console

	rails console --sandbox

Server 
	
	rails s

==Git

	git init
	git add .
	git commit -m ""
	git push remote master


==Heroku

	heroku create --stack-cedar
	git push heroku master
	heroku ps



