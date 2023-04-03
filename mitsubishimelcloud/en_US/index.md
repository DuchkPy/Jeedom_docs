---
title: Documentation Mitsubishi MELCloud plugin Jeedom
description: Documentation plugin Mitsubishi heat pump
logo: mitsubishimelcloud/mitsubishimelcloud_icon.png
---

# Description:

This plugin allows you to communicate with the Mitsubishi heat pumps that are connected to their MELCloud servers.

# Configuration:
When installing the plugin, the connection parameters must be entered in the plugin's configuration:
![configuration](./Configuration.png?raw=true)

Here is the order in which to fill in the information:
1. The email address and password used to log in to MELCloud (the application)
2. Save via the button on the `Configuration` line
3. Click on the `Retrieve MELCloud Token` button
4. Click on the `Retrieve MELCloud equipment` button

The application version available in the advanced section corresponds to the version of the MELCloud application. Currently, even with a version not up to date, it works. However, it is possible that this version may need to be updated in the event of a major overhaul by Mitsubishi.
So, as it stands, there is no need to change this value.

# Creating equipment:
In the configuration, after clicking on `Retrieve MELCloud equipment`, all the heat pump associated with this account are added to Jeedom.
If you have not performed this action, or if there are changes to the equipment in your home, the `Synchronize` button on the plugin's home page allows you to restart the process. Also, a cron runs this action regularly.

You only have to activate and associate each item with the right object in your Jeedom to find it (or not) on the dashboard.

# Widget:
Once created, each equipment will be visible (if requested) on the dashboard with the following design:
![widget](./Widget.png?raw=true)
I wanted to keep the design as close as possible to the MELCloud app to maintain the habits of people who already have it.

When sending a new value (mode, temperature, etc.) from Jeedom, small dots appear after the word "refresh", indicating the communication between Jeedom and your heat pump via the MELCloud servers. These disappear when the exchange is complete, and the entire widget is updated with the latest status values.

# Contribute:
If you detect a bug or want to suggest an improvement, don't hesitate to mention it on the forum (with the dedicated tag). You can also directly make a PR on [the repository of this plugin](https://github.com/DuchkPy/mitsubishimelcloud).

# Acknowledgements:
To the work initiated by MGeek for the reverse engineering on the MELCloud app [http://mgeek.fr/blog/un-peu-de-reverse-engineering-sur-melcloud](http://mgeek.fr/blog/un-peu-de-reverse-engineering-sur-melcloud) ([archive](https://web.archive.org/web/20220120005605/http://mgeek.fr/blog/un-peu-de-reverse-engineering-sur-melcloud)).
Then to the first plugin created by [Floman321](https://github.com/floman321/melcloud), which unfortunately is no longer up to date, that I forked to continue supporting Mitsubishi heat pump.

# License:
As desired by MGeek (see footer of his website), this plugin is licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/) license, so it is free.


# Changelog&nbsp;:
[Changelog](./changelog.md)