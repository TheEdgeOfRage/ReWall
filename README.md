# Rice script

A small script that pulls a wallpaper from https://reddit.com/r/earthporn , sets it as the wallpaper, extracts the colors and sets them in the terminal and i3

## Dependencies
[PRAW](https://github.com/praw-dev/praw) - Reddit api wrapper for python
[PyWal](https://github.com/dylanaraps/pywal/) - Script that generates a color palette from an image
[requests](https://github.com/requests/requests) - Python module for http requests, required for getting the images
[feh](https://feh.finalrewind.org/) - For setting the wallpaper on i3 (available in most package managers)

## Usage
1. Go to https://www.reddit.com/prefs/apps/ and click the `create app` button at the bottom
2. Fill in a name and redirect url (anything will do) and check the script radio button
3. Copy the id (3rd line, right under the name) and the secret into the rewall script in this repo

### Additional steps for i3 colors:
1. Copy your i3 config to base_config in the same folder
2. Open the base_config file from this repo and see where the colors are defined.
3. You'll have to either copy the blocks into your i3 base_config or adapt it so that it follows the same color variable names, as the variables will be prepended to the i3 conf that is generated.
