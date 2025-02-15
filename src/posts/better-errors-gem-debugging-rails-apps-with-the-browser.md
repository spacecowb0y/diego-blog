---
title: "Better Errors Gem: Debugging Rails apps with the browser"
path: "/better-errors-gem-debugging-rails-apps-with-the-browser"
date: "2013-01-21"
author: "Diego"
excerpt: "Since a long time the browser is not just an interface to surf the web."
tags: ["ruby_on_rails"]
coverImage: ../images/better_errors_rails_gem_example.png
---

If you are a front-end developer, I'm sure that firebug its your best friend while fighting with a CSS issue, or finding an error in your javascript, and many other debugging and monitoring tasks.

In my particular case, when I'm programming application based on Ruby on Rails, the browser doesn't offer me too much information when an error happens. That's where Better Errors comes to the rescue.

### What is Better Errors?

Better Errors is a gem developed by Charlie Somerville, and it purpose its to replace the classic built-in error page provided by Rails for something more interactive and usable, and adds some cool functionality like:

- Full stack trace
- Source code inspection for all stack frames (with hightlighting)
- Local and instance variable inspection
- Live REPL on every stack frame

### How do I integrate Better Errors on my Rails app?

That's easty. Just add it to your `Gemfile`, like this:

``` ruby
group :development do
  gem "better_errors"
end
```

And the best part is works with any Rack app, not just Rails.