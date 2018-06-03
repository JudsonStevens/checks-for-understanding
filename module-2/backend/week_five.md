### Week 5 Questions

Re-pull from this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!). 

Note: When you're done, submit a PR. 

### Week 5 Questions
1. How do we make flash messages display on a page?
  We use flash[:(type of notice)] in the controller and then we put an enumerable typically in the application view to display any flash messages on every page.

2. Where is cart information/temporary information usually stored?
  Inside the session.

3. What might be some reasons not to store a cart in our database? Are there any reasons why we would want to persist that information?
  I'm not sure of reasons to not store it in the database. Storing it in the database allows the cart to persist over sessions and can allow us to recall that cart for the user at any time in the future.

4. What is the purpose of the asset pipeline?
  The asset pipelines allows rails to compile all of the assets into a couple files so that it's not having to send responses to the browser for every single image or css file.

5. Why do we precompile our assets?
  Answer above.

6. What do each of the following tags do?

```ruby 
<%= stylesheet_link_tag "application" %>
<%= javascript_include_tag "application" %>
<%= image_tag "rails.png" %>
```
  The stylesheet link tag links the application stylesheet in our application to the current page. Ditto for the javascript. The image tag will make an HTML image tag and dipslay the rails picture.

7. What are some of the elements of a great read me? What are some of the benefits of taking the time to update a readme for our project?
  Well thought out directions on how to install and run your app. A guide to potential troubleshooting, and a list of helpful resources. This allows our users to know exactly how to download and run the app.

8. What are the top four accessibility issues that we as developers should be aware of?
  Not sure on this one.

9. `before_save` is an example of a what? Where in our Rails application would we find a `before_save`?
  That is a type of callback, and it would be typically in the model.

10. Given the following object, how would we create a scope for all users who are active?

```ruby 
User.create(name: "Happy", active: true)
```

  We could make a method in the application helper to ask if a user is active before displaying any information, and include that in our controllers.

11. What is the difference between a scope and a class method?


### Review Questions:  
12. Given the following hash:  

```ruby
{cart: {"17" => 4, "204" => 52, "29" => 22}}
```

  12a. How would you add item with id of 48 with a quantity of 4?  
    cart["48"] = 4
  12b. How would you increase the quantity of item 29?  
    cart["29"] += 1
  12c. How would you find out how many items your user is thinking about purchasing?   
    cart.values.sum
  
13. What is polymorphism? How does it relate to duck-typing? What are two ways you use this in everyday Rails applications? 
  Polymorphism has to do with the interface of an object. For example, we could have multiple animals that can all speak, but the method of speaking could be different in each. We use this in Rails when every controller has the same methods, but they do different things depending on the controller.
14. How would you clean the string "(630) 854-5483" to "630.854.5483"?  
  


### Self Assessment:
Choose One:
* I was able to answer every question without relying on outside resources *****
* I was able to answer most questions independently, but utilized outside resources for a few
* I was able to answer a few questions independently, but relied heavily on outside resources 

Choose One:
* I feel confident about the content presented this week ******
* I feel comfortable with the content presented this week
* I feel overwhelmed by the content presented this week
* I feel quite lost by the content presented this week
