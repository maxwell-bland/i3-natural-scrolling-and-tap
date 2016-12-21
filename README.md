# i3-natural-scrolling and tap-to-click
The above are two scripts that use an alternate method to enable natural scrolling and tap-to-click on machines running the i3 window manager. This was created after a realization that, for machines that do not use a synaptics touchpad, the easily googlable solutions to enable universal natural scrolling and tap-to-click are not applicable: these include modifying .Xmodmap (not universal) and using synclient (also not universal). 

# IMPORTANT NOTE!
The above scripts *may not work for your machine* and may require modifications, but hopefully only minor ones. You may have to _change the arguments to grep_ and the _format of the cut commands to grab the proper fields._ The hope is, however, that this is straight forward enough. It will certainly save you time if it works, and enable *universal* natural scrolling as well as the tap-to-click feature.

# How to Use

Save the scripts to some easily accessible folder. For me it is "~/.scripts/", and then add the following lines to the end of your i3 configuration file: "exec (path to script folder)/inverse-scroll.sh" and "exec (path to script folder)/tap-to-click.sh"

*Test the script before-hand! Make sure the values of $id, $natural_scrolling_id, and $tap_to_click_id are correct! This works on my computer but it may not work on yours out of the box!*

And that's it. hopefully it is straight-forward enough and provides a nice fix for those without synaptics touchpad drivers. 
