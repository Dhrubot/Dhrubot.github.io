---
layout: post
title:      "ERB, you beauty! "
date:       2020-06-08 02:49:02 +0000
permalink:  erb_you_beauty
---

As we are approaching towards Ruby on Rails, this past project week was all about Sinatra and ActiveRecord. Along my way to make a basic sinatra web app, I’ve had the pleasure to meet Bootstrap too. Don’t get me wrong, all of these frameworks and interfaces are very powerful and albeit makes a software developers life so much easier! I was amazed the way these tools simplifies a lot of the crucial tasks! Take password validations for an instance. When I didn’t know better, I thought what kind of magic are these programmers doing that their programs know that I haven’t used a symbol for my password! Then I’ve got my hands on ActiveRecord and it’s awesome validation options! But I am gonna write today about how I made a navbar with hidden items using the ERB.

When we talk about responsive functionality of a webpage, immediately Javascript comes to mind. So when this project came along I was thinking that I will probably have to build a very static site since I don’t know Javascript. But then, came along ERB or Embedded Ruby. ERB lets you embed Ruby code in your html and it is very powerful. For my project I decided to make a navbar with collapsible menu items which would be changing depending on if the user is logged in or not.
This is from a guest’s perspective
![](https://miro.medium.com/max/834/1*OB7HCg9Zv1MjNkS8_olkug.png)

I’ve used bootstrap to achieve the navbar and it’s contents. Then used ERB to make it more dynamic in a way that when a user logs in he can hav access to more nav items.
Nav items after logging in with a dropdown menu
This is the user’s personalized menu.
![](https://miro.medium.com/max/314/1*FjncIbDNzDFnxL4YcMqh2A.png)
![](https://miro.medium.com/max/156/1*iqjbaxcxk1rYFtZWZQn0Sg.png)

To achieve this function, first I made sure to enable and set sessions from my Application Controller and then in my User model I set the session[:id] to the user’s id upon logging in. Then I wrote a helper method in my Application Controller which sets a current user based on the session id if the user logs in and if there is a session[:id] is present. After all these ERB just made it too easy. All I had to do was to implement a simple if and else statments in my html file and based on the current_user condition my navbar became dynamic!

In times I felt lost but with the awesome resources that are available through Flatiron School Faculty, my peers and the internet , in the end this turned out to be a really interesting project, I had the chance to learn a ton of materials and I am certainly looking forward for the next one!
