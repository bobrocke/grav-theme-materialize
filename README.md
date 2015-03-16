# Materialize

![Materialize](screenshot.jpg)

Materialize is a [Grav](http://github.com/getgrav/grav) theme that is based on the [Materialize framework](http://materializecss.com).

# Installation

Installing the Materialize theme can be done in one of two ways. Our GPM (Grav Package Manager) installation method enables you to quickly and easily install the theme with a simple terminal command, while the manual method enables you to do so via a zip file.

## GPM Installation (Preferred)

The simplest way to install this theme is via the [Grav Package Manager (GPM)](http://learn.getgrav.org/advanced/grav-gpm) through your system's Terminal (also called the command line).  From the root of your Grav install type:

    bin/gpm install materialize

This will install the Materialize theme into your `/user/themes` directory and the required Materializer plug-in into your `/user/themes` directory, both within Grav. Its files can be found under `/your/site/grav/user/themes/materialize` and `/your/site/grav/user/plugins/materializer`.

## Manual Installation

To install this theme, just download the zip version of this repository and unzip it under `/your/site/grav/user/themes`. Then, rename the folder to `materialize`. You can find these files either on [GitHub](https://github.com/getgrav/grav-theme-materialize) or via [GetGrav.org](http://getgrav.org/downloads/themes).

You should now have all the theme files under

    /your/site/grav/user/themes/materialize

And then you must download the zip version of the Materializer plug-in repository and unzip it under `/your/site/grav/user/plugins`. Then, rename the folder to `materializer`. You can find these files either on [GitHub](https://github.com/getgrav/grav-plugin-materializer) or via [GetGrav.org](http://getgrav.org/downloads/plugins).

You should now have all the plugin files under

    /your/site/grav/user/plugins/materializer

>> NOTE: This theme is a modular component for Grav which requires the [Grav](http://github.com/getgrav/grav), [Error](https://github.com/getgrav/grav-theme-error) and [Problems](https://github.com/getgrav/grav-plugin-problems) plugins.

# Updating

As development for the Materialize theme continues, new versions may become available that add additional features and functionality, improve compatibility with newer Grav releases, and generally provide a better user experience. Updating Materialize is easy, and can be done through Grav's GPM system, as well as manually.

## GPM Update (Preferred)

The simplest way to update this theme is via the [Grav Package Manager (GPM)](http://learn.getgrav.org/advanced/grav-gpm). You can do this with this by navigating to the root directory of your Grav install using your system's Terminal (also called command line) and typing the following:

    bin/gpm update materialize

This command will check your Grav install to see if your Materialize theme is due for an update. If a newer release is found, you will be asked whether or not you wish to update. To continue, type `y` and hit enter. The theme will automatically update and clear Grav's cache.

## Manual Update

Manually updating Materialize is pretty simple. Here is what you will need to do to get this done:

* Delete the `your/site/user/themes/materialize` directory.
* Downalod the new version of the Materialize theme from either [GitHub](https://github.com/getgrav/grav-theme-materialize) or [GetGrav.org](http://getgrav.org/downloads/themes#extras).
* Unzip the zip file in `your/site/user/themes` and rename the resulting folder to `materialize`.
* Clear the Grav cache. The simplest way to do this is by going to the root Grav directory in terminal and typing `bin/grav clear-cache`.

>> Note: Any changes you have made to any of the files listed under this directory will also be removed and replaced by the new set. Any files located elsewhere (for example a YAML settings file placed in `user/config/themes`) will remain intact.

# Setup

If you want to set Materialize as the default theme, you can do so by following these steps:

* Navigate to `/your/site/grav/user/config`.
* Open the **system.yaml** file.
* Change the `theme:` setting to `theme: aterialize`.
* Save your changes.
* Clear the Grav cache. The simplest way to do this is by going to the root Grav directory in Terminal and typing `bin/grav clear-cache`.

Once this is done, you should be able to see the new theme on the frontend. Keep in mind any customizations made to the previous theme will not be reflected as all of the theme and templating information is now being pulled from the **materialize** folder.

It is possible to add top level menu items via entries in `site,yaml` in this form:

```
menu:
  - text: Item 1
    url: http://
    icon: icon-name

  - text: Item 2
    url: http://
    icon: icon-name
```

The url fields is mandatory if the menu structure is used. The menu text is optional, allowing for an icon-only menu item. The icon field is also optional, but if present, refers to an icon in the [Design Icon Font](http://materialdesignicons.com).
