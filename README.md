# twist_mux

This is a multiplexer for [geometry_msgs/Twist](http://docs.ros.org/api/geometry_msgs/html/msg/Twist.html) topics and [std_msgs/Bool](http://docs.ros.org/api/std_msgs/html/msg/Bool.html) locks with priorities.

See [documentation](http://wiki.ros.org/twist_mux).

## Usage for the mobile robot:
This multiplexer allows for multiple sources to provide (linear/angular) velocity commands for the mobile robot. In particular, this allows the navigation node to provide commands via the `cmd_vel_mux/input/nav_vel` topic and the keyboard teleoperation node to provide commands via the `mattbot_teleop/cmd_vel` topic. The teleoperation has precedence over the navigation commands.

To adjust the preferences or add additional sources for the multiplexer, please edit the [config/twist_mux_topics.yaml](./config/twist_mux_topics.yaml) file.

## License
This package is licensed under the Apache License 2.0. See the [LICENSE](LICENSE.txt) file for the full license text.

**Authors**:
- Enrique Fernandez
- Siegfried-A. Gevatter Pujals

**Edited By**:
- Matthew Sato, Stanford University Engineering Informatics Group