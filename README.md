# Getting-Started-with-Rails-blog-
Getting Started with Rails (blog)

3.2 Creating the Blog Application
	$ rails new blog
	$ cd blog

4.2 Say "Hello", Rails
	$ bin/rails generate controller welcome index

4.3 Setting the Application Home Page
	<h1>Hello, Rails!</h1>
	root 'welcome#index' //file: config/routes.rb

5 Getting Up and Running
	resources :articles  //file: config/routes.rb

5.1 Laying down the ground work
	$ bin/rails generate controller articles 
	//file: app/controllers/articles_controller.rb
		def new   
		end

5.2 The first form
	app/views/articles/new.html.erb

5.3 Creating articles

5.4 Creating the Article model
	$ bin/rails generate model Article title:string text:text

5.5 Running a Migration
	$ bin/rake db:migrate

5.6 Saving data in the controller

5.7 Showing Article

5.7 Showing Articles

5.8 Listing all articles

5.9 Adding links

5.10 Adding Some Validation

5.11 Updating Articles

5.12 Using partials to clean up duplication in views

5.13 Deleting Articles

6 Adding a Second Model

6.1 Generating a Model
	$ bin/rails generate model Comment commenter:string body:text article:references

6.2 Associating Models

6.3 Adding a Route for Comments  
	//file: config/routes.rb
	resources :articles do
  		resources :comments
	end
