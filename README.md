prototype-rails provides Prototype, Scriptaculous, and RJS on Rails 3.1
and later.

---

**Note from @anamba**: Minimal changes have been made to allow this gem to continue working on newer Rails versions, up to 5.2. Obviously, you should try to update your application to use JQuery or some other active JS framework (or perhaps none at all!), but if you cannot, this fork should help you out. No guarantees, of course. Some functionality may be broken.

This repository was rebased on 2019-04-16 to make it clear that it is not behind [upstream](https://github.com/rails/prototype-rails) in any way. Apologies for any inconvenience. No further upstream changes are expected, so there should be no future rebases, either.

Original README follows.

---

Prototype and Scriptaculous are pulled in by the asset pipeline, so you don't
need to copy the source files into your app. You may reference them in your
s app/assets/javascripts/application.js:

    //= require prototype
    //= require prototype_ujs
    //= require effects
    //= require dragdrop
    //= require controls

prototype-rails supports RJS debugging. RJS responses are wrapped to catch
exceptions, alert() them, and re-raise the exception. Debugging is disabled by
default. To enable in development, set `config.action_view.debug_rjs = true`
in config/environments/development.rb.

---

## Support for Rails 4.1 and above

Unfortunately, due to limited manpower and resources, the Rails core team has
not been able to confirm if this gem currently works with Rails 4.1 and above.
If you have found any problems while upgrading your application, please report
them at the [issue tracker](https://github.com/rails/prototype-rails/issues),
or better yet, submit patches by sending a [pull request](https://github.com/rails/prototype-rails/pulls).

In any case, this gem will *NOT* be officially supported on Rails 5.0 and above.
