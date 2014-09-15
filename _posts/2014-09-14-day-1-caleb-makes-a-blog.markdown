---
layout: post
title:  "Day 1 - Caleb Makes a Blog"
date:   2014-09-14
tags: [blog, meta]
---

Hello, my name is Caleb. The posts you'll read in this blog are here for two reasons: accountability and documentation. I want to hold myself accountable. To me, to you, and to my game. I will post my progress every day and I will do something every day, no matter how tiny.

Second, I will try to teach you a little something every day. I realize that I will make a lot of mistakes along this journey, and that's okay, because I will write about them. And hopefully, when someone in the future searches Google with some strange error, my blog will pop up and help them out.

I think it's important to say why I want to create a game, especially when I'm about to commit so much time to it. The first game I made was in high school. I created a snake clone in VB.NET. Besides that game and the port I made to C# and XNA, I have not finished a game in the five years since. I have tried before and failed many times, so this time I'm trying something new. Hopefully this will work.

But that's enough about the meta of this blog. It's time for this day's progress!

--------

## Setting up a Jekyll Blog

I decided on a Jekyll blog, partly because I've made one before. I don't like how I have to type my posts in markdown on my desktop and have a shell serving the html in order to preview it, but having a static blog has a lot of benefits. For one, you only serve up text files and css, so your blog scales tremendously.

To set up a Jekyll blog, I followed [this tutorial](http://jekyll-windows.juthilo.com/). It walks you through installing up Ruby, Ruby DevKit, and the Jekyll gem on Windows.

After I had my prerequisites out of the way, I ran `jekyll new calebmakesagame`. I then added the directory to git using GitHub for windows and published it. I deleted my `master` branch and switched over to `gh-pages`.

After that, I had to change some stuff in my `_config.yml` file. Note that this is for **GitHub Project pages**. GitHub profile or organization pages aren't hosted under a subdirectory, so you don't need to mess with `baseurl`.

    baseurl: "/calebmakesagame"
    url: "http://cable729.github.io/calebmakesagame"

Of course, don't forget to look at the rest of the config and change the description, title, and author details of the blog.

## Writing a Post

Creating a post is easy-peasy. All you have to do is add a `.markdown` file to the `/_posts` directory, using a name such as `2014-09-14-day-1-caleb-makes-a-blog.markdown`. You can set meta parameters on the top of the file. For instance:

    ---
    layout: post
    title:  "Day 1 - Caleb Makes a Blog"
    date:   2014-09-14 13:19:30
    categories: blog meta
    ---

Markdown is interpreted the same as pretty much everywhere, so if you've used a markdown editor before, you'll feel right at home.

When you want to preview your work, open a prompt in the `calebmakesagame` directory and run

    > jekyll serve --watch --baseurl ''

After you're satisfied, push your code to GitHub and it will compile your site.

That's it guys. Hope you learned something. Comments may be coming soon if you'd like to ask questions, until then you can reach me on twitter [@cable729](http://twitter.com/cable729).

See you tomorrow!

<!-- You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve --watch`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll’s dedicated Help repository][jekyll-help].

[jekyll]:      http://jekyllrb.com
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-help]: https://github.com/jekyll/jekyll-help
 -->