---
layout: post
title:  "Jekyll to GitHub"
date:   2014-08-28 01:10:11
categories: jekyll github
---
First, you create an account on GitHub.
Then create a repo called `githubusername.github.io`.
Assuming you're using Linux/Unix/Mac, you require [Ruby][ruby], [RubyGems][rubygems] and [NodeJS][nodejs].

Open terminal, follow the commands.
Install with RubyGems
{% highlight ruby %}
$ gem install jekyll
{% endhighlight %}

Jekyll - Basic usage

{% highlight ruby %}
$ jekyll new githubusername.github.io
# => Creates githubusername.github.io folder in the current folder

$ cd githubusername.github.io
# => changes directory to githubusername.github.io

$ jekyll build
# => The current folder will be generated into ./_site

$ jekyll serve
# => A development server will run at http://localhost:4000/

$ jekyll serve --watch
# => Same as `jekyll serve`, 
#    but watch for changes and regenerate automatically.
{% endhighlight %}

You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve --watch`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

After completion of post writing,
you can deploy your site to github.
{% highlight ruby %}
$ git add --all
# => Adding all files and folders in the current folder to git.

$ git commit -m "Jekyll theme added."
# => Commiting git with a message.

$ git push
# => You are done.
{% endhighlight %}

Open browser, check out your website, `githubusername.github.io`.

Check out the [Jekyll docs][jekyll] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll’s dedicated Help repository][jekyll-help].

[ruby]:		http://www.ruby-lang.org/en/downloads/
[rubygems]:	http://rubygems.org/pages/download
[nodejs]:	http://nodejs.org/

[jekyll]:      http://jekyllrb.com
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-help]: https://github.com/jekyll/jekyll-help
