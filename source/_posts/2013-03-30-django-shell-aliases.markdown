---
layout: post
title: "Django Shell Aliases"
date: 2013-03-30 09:07
comments: true
categories: django zsh 
---

Writing `python manage.py runserver` all day long can get tedious. Even `./manage.py runserver` sucks. A coworker of mine, [James](https://github.com/jameskeane), suggested to create a shell alias. James maps `@` to `python manage.py` so he can just type `@ runserver`.

I have decided to take this a step farther and shorten up all of the common `manage.py` commands. Here is a snippet from my `.zshrc`:

```
## Django Aliases
alias @="python manage.py"
alias @r="python manage.py runserver"
alias @sh="python manage.py shell"
alias @db="python manage.py sync_db"
alias @m="python manage.py migrate"
alias @su="python manage.py createsuperuser"
```

