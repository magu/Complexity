## Complexity

Complexity is a quick and dirty mod of the Simplicity watch face for Pebble&mdash;included in the SDK&mdash;which adds Week Day and Week Number to the main screen.

### Building the watch face

First, create a new project with the `create_pebble_project.py` script included in the [Pebble SDK](http://developer.getpebble.com).

    cd <parent dir of project root>

    /<sdk_path>/tools/create_pebble_project.py --symlink-only /<sdk_path>/sdk/ complexity

    cd complexity

    ./waf configure build
