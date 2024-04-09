# Sentry Robot
Robomaster repo for sentry robot modeling, autonomous navigation stack, and other fun things

## TO RUN NAV2:

  In one terminal:
  ```
   colcon build
   source install/setup.bash
   ros2 launch sentry sentry_simulation.launch.py
  ```
...Wait for simulation to boot up completely...

  Open a separate terminal:
  ```
   colcon build
   source install/setup.bash
   ros2 launch sentry sentry_navigation.launch.py
  ```

...Wait for AMCL message in 2nd terminal...

  IN RVIZ, click set 2d pose at the top and click/drag arrow to match pose of robot in Gazebo. Then click Nav2 Goal and click and drag an arrow somewhere for path planning to that goal orientation.

  sentry/config/navigation.yaml contains all parameters for NAV2/AMCL

