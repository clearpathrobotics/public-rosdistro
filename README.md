public-rosdistro
================

A [REP 141][1] repository which governs the packages published
publicly to [packages.clearpathrobotics.com][2].


bloom setup
-----------

To have bloom produce a pull request directly to here, run:

    export ROSDISTRO_INDEX_URL=https://raw.githubusercontent.com/clearpathrobotics/public-rosdistro/master/index.yaml
    bloom ...

rosdep setup
------------

To resolve rosdep keys for internal builds, run:

    sudo wget https://github.com/clearpathrobotics/public-rosdistro/raw/master/rosdep/50-clearpath.list -O /etc/ros/rosdep/sources.list.d/50-clearpath.list
    rosdep update

[1]: http://ros.org/reps/rep-0141.html
[2]: http://packages.clearpathrobotics.com/
