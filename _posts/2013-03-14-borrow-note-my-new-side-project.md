---
layout: post
title: Borrow Note - my new side project
---

Over the last year or so I have learned how hard it is to build a business out of an online product or service. I've learned this through the experiences of friends, co-workers and groups such as the [Business Bootstrap Club](http://bootstrapbusinessclub.co.uk/).

So a couple of months ago I decided that instead of waiting until I had the financial flexibility and time to invest in creating a bootstrapped business, I should instead consider the ideas I have for web apps as side projects. This way there is little pressure for the product to grow big, or even succeed, and I can enjoy the development process in my own limited time.

So I created Borrow Note: [http://www.borrownote.com](http://www.borrownote.com)

![Screen_shot_2013-03-05_at_16.23.57](http://s3.amazonaws.com/bobob_prod/images/medium/16/Screen_Shot_2013-03-05_at_16.23.57.png?1362500673 "Borrow Note")

The idea came from the fact that my wife and I forget who we've lent stuff too, and we borrow things quite reguilarly from friends and family. To be reminded who borrowed what and to see if any friends have a drill, for example, which I could borrow would be very useful, and I thought such a tool might be useful to others.

Seeing Borrow Note as a side project means I can experiment with different Ruby Gems, Heroku Add-ons and coding techniques, which I've really enjoyed. So I've used [Foundation](http://foundation.zurb.com/) as the visual framework instead of Twitter's Bootstrap which I've used previously. I also wanted to use [Formtastic](https://github.com/justinfrench/formtastic) instead of [Simple Form](https://github.com/plataformatec/simple_form), but I discovered Simple Form integrates much better with Foundation, especiallly with the inline errors which Rails produces when form data is not valid. I had heard of a [Markerb](https://github.com/plataformatec/markerb), a gem which uses a single Mardown file to create both the HTML and Text multiparts of an email, so I've used that to see how good it is.

I decided to create a very basic reminder service, then get some feedback before I add further features. The feedback I've had has confirmed my thoughts on allowing users to create accounts to track multiple items, with additional features, such as specifying a particular date for the reminder email to be sent, and to see what friends on the site have available to borrow.

Starting Borrow Note has certainly satisfied my desire to create and experiment, and has provided an alternative to watching nonsense in my evenings!