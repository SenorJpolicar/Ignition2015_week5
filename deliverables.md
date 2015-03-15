#### Deliverables for week 5 Rails MVC
##### Odin Project Routing Guide Questions:
- What is the "Root" route? It tell rails which which controller and action to map the route to.          
- What are the seven RESTful routes for a resource? 
    1. GET all the posts (aka "index" the posts 2.GET just one specific post (aka "show" that post) 3. GET the page that lets you create a new post (aka view the "new" post page) 4. POST the data you just filled out for a new post back to the server so it can create that post (aka "create" the post)  5. GET the page that lets you edit an existing post (aka view the "edit" post page)  
    6. PUT the data you just filled out to edit the post back to the server so it can actually perform the update (aka "update" the post) 
    7. DELETE one specific post by sending a delete request to the server (aka "destroy" the post)

- Which RESTful routes share the same URL but use different verbs?get "/posts/:id" => "posts#show", put "/posts/:id" => "posts#update", delete "/posts/:id" => "posts#destroy"  
- How do you specify an ID or other variable in a route? you prepend it with a colon. 
- How can you easily write all seven RESTful routes in Rails? you use a sample controller. 
- What is the Rails helper method that creates the HTML for links?  edit_post  GET  /posts/:id/edit(.:format)  posts#edit

##### Odin Project Views Guide Questions:
- What is a layout? the file that holds the head tags and the DOCTYPE and other basic structure that is in all pages. 
- What's the difference between a "view template" and a "layout"? The view template is not the whole web page. 
- What is a "Preprocessor"?  It's a special way of executing ruby code inside your HTML.
- Why are preprocessors useful? it alows you to use ruby inside your html.  
- How do you make sure a preprocessor runs on your file? you put it in your ruby tags.
- What's the outputted filetype of a preprocessed *.html.erb file? What about a *.css.scss file? turns into regular html and regular CSS. 
- What is the difference between the <%= and <% tags? <%= will display whatever is inbtween the tags. <% will jsut run the code but wont show anything in the html. 
- What is a view partial? it is a way tpo break things apart and make your code and make it easier to read and keep organized. It also lets you reuse certain common paterns. 
- How do you insert a partial into your view?you use two names that are in the original file name. 
- How can you tell that a view file is a partial? the underscores ? 
- How do you pass a local variable to a partial? you drop the @ sign. 
- What's the magical Rails shortcut for rendering a User? A bunch of Users?
- <h1>Users</h1>
    <ul>
      <% @users.each do |user| %>
        <%= render user %>     
      <% end %>
    </ul>

 <h1>Users</h1>
    <ul>
      <%= render @users %>
    </ul>
- What are asset tags and why are they used? they locate the files based on the names you gave them and render and give them the proper html tag. 

##### Link to Odin Project Basic Routes, Views and Controllers repo: [my odin repo](<linkhere>)
##### Link to Hartl's Rails Tutorial Chapter 5 repo: [my hartl's repo](https://github.com/SenorJpolicar/testy-.git)
