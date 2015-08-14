Apple Pie
=========

Apple Pie is a helper script to make easy launchers for websites in chrome's
app mode, each with their own profile.  This accomplishes a few things:

* App mode lets webapps behave more like a normal application on the desktop
  for things like alt-tab, iconography, etc.

* Separate profiles mean that different apps won't be able to track your
  behavior from site to site.

* Separate profiles let you be logged into multiple google/twitter/facebook
  accounts at once

* Easy launching from ~/bin, either from the command line or [gbashrun](https://github.com/jewel/gbashrun)

* Fine control of profiles lets you share profile in some cases.  For example,
  I have `gcal`, `gmail`, `gdrive` shortcuts for work.


Installation
------------

Copy or symlink `apple-pie` into your path.

Install ruby and curl.

Install the `pismo` gem.  This is used to download site icons.


Usage
-----

Arguments are:

* `friendly_name`: Name that's visible in some places in gnome
* `url`: Start URL.  Derived from friendly name if not given
* `profile`: Unique name for the profile.  Derived from friendly name if not
  given


Copy apple-pie to ~/bin.  Create shell scripts like:

```sh
#!/bin/sh
apple-pie Pandora
```

A more advanced setup would look like this:

```sh
#!/bin/sh
apple-pie 'Work Calendar' https://calendar.google.com work-google
```

Contributing
------------

Pull requests welcome!
