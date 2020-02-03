+++
date = 2012-02-07T00:00:00Z
draft = true
layout = "post"
title = "Modifying Hugo Themes Fonts"

+++
<div class="message"> Hello! This is my first blog post on data science, R, analytics and blogdown. </div>

Hello, data friends! I spent the past weekend diving into blogdown after rstudio::conf and I'm excited to share my site [https://gabe.rbind.io/](https://gabe.rbind.io/ "https://gabe.rbind.io/") with the community. I experienced a number of frustrating and satisfying moments along way, while reading up on how to modify CSS in order to change font types from the [Hyde Hugo Theme](https://themes.gohugo.io/hyde/) that I had decided to use. 

I had initially thought that changing font types would be an easy task. It **was**, _but _it took me a while to find documentation that addressed the issue I was facing. For reference, here's the Hugo discourse page that I found most helpful [https://discourse.gohugo.io/t/help-with-customizing-beautifulhugo-theme/16371](https://discourse.gohugo.io/t/help-with-customizing-beautifulhugo-theme/16371 "https://discourse.gohugo.io/t/help-with-customizing-beautifulhugo-theme/16371")

## Heading

Vivamus sagittis lacus vel augue rutrum faucibus dolor auctor. Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit. Morbi leo risus, porta ac consectetur ac, vestibulum at eros.

### Code

Cum sociis natoque penatibus et magnis dis `code element` montes, nascetur ridiculus mus.

{% highlight js %}
// Example can be run directly in your JavaScript console

// Create a function that takes two arguments and returns the sum of those arguments
var adder = new Function("a", "b", "return a + b");

// Call the function
adder(2, 6);
// > 8
{% endhighlight %}

Aenean lacinia bibendum nulla sed consectetur. Etiam porta sem malesuada magna mollis euismod. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa.

### Gists via GitHub Pages

Vestibulum id ligula porta felis euismod semper. Nullam quis risus eget urna mollis ornare vel eu leo. Donec sed odio dui.

{% gist 5555251 gist.md %}

Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Nullam quis risus eget urna mollis ornare vel eu leo. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec sed odio dui. Vestibulum id ligula porta felis euismod semper.

***

I'll be writing more about my blogdown journey in the coming days. Any questions, or suggestions on what to tackle? <a href="https://twitter.com/gabegarcia15">Tweet me. </a>