![phpQGISrepository](https://gitlab.com/GIS-projects/phpQGISrepository/raw/master/logo.png)

# phpQGISrepository
phpQGISrepository is a simple PHP script to create a repository for <a href="http://qgis.org">QGIS</a> Python plugins.


## Good to know
* The script has **no settings**.
* The script is **ready to go**.
* The script needs **no database**.
* As long as your server can handle **PHP**-scripts you can use this on the internet or on an intranet.
* Make sure the **metadata.txt** is filled in correct in the QGIS Python Plugin zip-files.
* The script uses QGIS 3.x as default minimum and maximum version, but can also be used for QGIS 2.x, if the metadata.txt file of your plugin has the correct information.

## Why would I need my own repository?
* If you plan to share your plugins with the worldwide QGIS community, **you don't need it**. In that case use the official [QGIS Python Plugins Repository](https://plugins.qgis.org/plugins/plugins.xml).
* If you make plugins that are only intended for a limited number of QGIS users, **you can use this simple script** to create your own repository. 

## Demo
You can find a demo of the script on https://plugins.stuyts.xyz.

## How to install
* Download the latest release of phpQGISrepository from [GitLab](https://gitlab.com/GIS-projects/phpQGISrepository/tags).
* Upload all files inside the downloaded archive file to your server that can handle PHP scripts.
* Upload your valid QGIS Python Plugin zip-files to the 'downloads' subfolder. It already contains an example plugin. You can delete this example if you want. **Make sure the name of the zip-file is the same as the main directory in the zip-file: for example if the main directory in your zip-file is called MyPlugin, your zip-file should be named MyPlugin.zip.**
* Have a drink and enjoy your newly installed repository.

## How to use your repository
* In your browser go to the url of the main folder you installed the script in. (This is the same url you should add in QGIS)
* Add the repository to QGIS: "Plugins" - "Manage and install plugins..." - "Settings" - "Add...". (If you make QGIS plugins you probably already knew where to add a custom repository)

## Did you make some customisations to the plugins_bootstrap.xsl or plugins_v1.xsl files?
* Create a fork of this repository
* Add the xsl-file with an alternative name like *plugins_example_flashygreen.xsl* to your fork
* Create a pull request to this repository.  

This way they can be an example for other users.

## How do you make a plugin?
* More information on this topic can be found at http://docs.qgis.org/3.4/en/docs/pyqgis_developer_cookbook/plugins.html.

## This script is used by:
* [My demo site](https://plugins.stuyts.xyz)
* [Circet](http://web-dev.circet.fr/phpQGISrepository-master/)

If you use this scripts and you want your site listed above, please send a link to <a href="mailto:info@stuyts.xyz">info@stuyts.xyz</a>.
