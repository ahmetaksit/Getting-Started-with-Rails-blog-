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
