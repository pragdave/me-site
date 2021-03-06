---
layout: post
title: "A Simple Elixir Macro"
date: 2014-11-05
comments: true
tags: [programming, elixir]
---

### An Elixir Version of Rails' `returning`

A few days ago I was writing some code where just about every function ended

``` elixir
def func1 do
  # really cool code…
  result = do_some_calculation(...)
  Logger.info "func1 → #{result}
  result
end
```

(OK, so the actual code was more compelling than this).

I hated the use of the temporary result variable, so ended up writing an implementation of the Ruby on Rails `returning` method. The resulting macro was so concise and (I think) elegant, I thought I'd share:

<iframe width="560" height="315" src="//www.youtube.com/embed/LsLWezjV9Fo" frameborder="0" allowfullscreen></iframe>




