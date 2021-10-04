# ROS2 package with messages for the prophesee event based camera
The message layout is kept the same as in the original ROS1 message.

## How to build and install as symlink while exporting compile commands
```
colcon build --packages-select prophesee_event_msgs --symlink-install --cmake-args -DCMAKE_BUILD_TYPE=RelWithDebInfo -DCMAKE_EXPORT_COMPILE_COMMANDS=ON
```

## How to run linter and see what failed
```
colcon test --packages-select prophesee_event_msgs
colcon test-result --verbose
```

## License
This ROS2 version of ``prophesee_event_msgs`` is released under the [Apache-2 license](LICENSE).
