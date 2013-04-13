## Complexity

![Action shot](https://raw.github.com/magu/Complexity/master/releases/complexity-1.0.png)

Complexity is a quick and dirty mod of the Simplicity watch face for Pebble which adds Week Day and Week Number to the main screen.

### Building the watch face

First, create a new project with the `create_pebble_project.py` script included in the [Pebble SDK](http://developer.getpebble.com).

    cd <parent dir of project root>

    /<sdk_path>/tools/create_pebble_project.py --symlink-only /<sdk_path>/sdk/ complexity

    cd complexity

    ./waf configure build

### Install the watch face using libpebble

First, make sure [libpebble](https://github.com/pebble/libpebble) is set up and running properly. Then:

    /<libpebble_path>/p.py --pebble_id <PEBBLE_ID_OR_MAC_ADDRESS> --lightblue load complexity-1.0.pbw
