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
