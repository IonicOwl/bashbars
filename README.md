# bashbars
Customisable resource bars for your MOTD

![bashbars_preview](https://github.com/IonicOwl/bashbars/blob/main/bashbars_banner.png?raw=true)

A portable and easily customisable way to add basic resource information to your MOTD, or run it by itself.


## Installation
Grab the sample file and save it to your machine.
Make sure it has execute permissions.
Run the script or add it to your MOTD.


## Basic Setup
You won't need to touch the bulk of the script, however at the bottom of the file, you can specify which volume(s) you wish to show in list format.
```
# List devices (function, device, threshold%)
spacer
membar memory 90
membar swap 90
spacer
volbar / 90
volbar /home 90
volbar /srv 90
volbar /var 90
volbar /usr 90
spacer
```

Memory and swap are already set up.  You can change the threshold percentage (set to 90% in the sample) as per your requirements.
Volumes can be added or removed as needed.  Just use `volbar` to specify a volume, followed by the volume name, then the threshold percentage.
The threshold percentage is the value that the bar will change to the specified alert colour.

You can use a `spacer` to separate groups of items.


## Further Customisation
You can change most visual attributes within the first few lines of the script, including colours, bar and column widths, segment characters.  You can even define custom width profiles to suit your terminal size.
