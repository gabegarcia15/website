+++
date = 2020-06-07T23:00:00Z
draft = true
layout = "post"
title = "Let's Get Rid of Right Joins"
weight = 1

+++
Back when I was first learning SQL, I was confused by the different types of joins.

<iframe src="[https://giphy.com/embed/3o7btZ1Gm7ZL25pLMs](https://giphy.com/embed/3o7btZ1Gm7ZL25pLMs "https://giphy.com/embed/3o7btZ1Gm7ZL25pLMs")" width="480" height="270" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="[https://giphy.com/gifs/reactionseditor-3o7btZ1Gm7ZL25pLMs](https://giphy.com/gifs/reactionseditor-3o7btZ1Gm7ZL25pLMs "https://giphy.com/gifs/reactionseditor-3o7btZ1Gm7ZL25pLMs")">via GIPHY</a></p>

<div class="message"> What is the difference between a right join and a right outer join? </div>

<div class="message"> When do I use a left join versus a right join? </div>

<div class="message"> How do I complete the ON statement within a JOIN </div>

ON Orders.CustomerID = Customers.ID?

I had initially thought that changing font types would be an easy task. It **was**, _but_ it took me a while to find documentation that addressed the issue I was facing. For reference, here's the Hugo discourse page that I found most helpful [https://discourse.gohugo.io/t/help-with-customizing-beautifulhugo-theme/16371](https://discourse.gohugo.io/t/help-with-customizing-beautifulhugo-theme/16371 "https://discourse.gohugo.io/t/help-with-customizing-beautifulhugo-theme/16371")

## Copypaste

Assuming that the reader's theme and website are already up and running and that the issue centers around modifying an existing theme, copypasting comes to the rescue. I read a number of posts talking about themes and [submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules), which I won't talk about in this post. It is a lot and I'm not sure if it is the best approach to configuring a site's layout.

My approach was much simpler.

**1) Find a font you like** [here](https://fonts.google.com/).

**2) Copypaste.** Copy the actual css file as is from the theme and paste it into the projectname/static/css folder. If the folder does not already exist, then create one. Hugo's content structure is hierarchical, so the hyde.css file I had placed in projectname/static/css/**hyde.css** will override projectname/themes/hyde/static/css/**hyde.css**. Also note that not all css files need to be included. In my case, I only overrode one css file and the rest remained located in projectname/themes/hyde/static/css/

**3) Update** hyde.css file I had placed in projectname/static/css/ with new font type. These two references already explain well how to make the update, so I won't be going into detail.

References:

* [https://www.rostrum.blog/2018/11/29/fontface-lithium/](https://www.rostrum.blog/2018/11/29/fontface-lithium/ "https://www.rostrum.blog/2018/11/29/fontface-lithium/")
* [https://tc.rbind.io/post/2018/02/15/how-to-use-web-fonts-in-blogdown/](https://tc.rbind.io/post/2018/02/15/how-to-use-web-fonts-in-blogdown/ "https://tc.rbind.io/post/2018/02/15/how-to-use-web-fonts-in-blogdown/")

**4) Test.** I published my website using Netlify and confirmed that the changes were successfully completed. I was also able to get an [rbind.io](https://github.com/rbind/support/issues "rbind.io") domain thanks to the team behind the rbind project. Anyone can get one for free, just remember to write one blog post or create one web page after getting the rbind.io subdomain!

***

I'll be writing more about my blogdown journey in the coming days. Any questions, or suggestions on what to tackle next? <a href="https://twitter.com/gabegarcia15">Tweet me. </a>