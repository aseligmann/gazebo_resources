# gazebo_resources

A collection of gazebo models and worlds

Based on RotorS resources, with added custom models

Add the following lines to `~/.bashrc`:
```bash
export GAZEBO_MODEL_PATH=$GAZEBO_MODEL_PATH:~/gazebo_resources/models
export GAZEBO_RESOURCE_PATH=$GAZEBO_RESOURCE_PATH:~/gazebo_resources/worlds
```

## Update Gazebo

It is recommended to upgrade Gazebo to the latest 9.X version.
This can be done by following these instructions: http://gazebosim.org/tutorials?cat=install&tut=install_ubuntu&ver=9.0#Alternativeinstallation:step-by-step

After updating, you will likely get an error along the lines of  
`gazebo: symbol lookup error: /usr/lib/x86_64-linux-gnu/libsdformat.so.6: undefined symbol: _ZTIN8ignition4math2v45ColorE`

This can be fixed by updating/reinstalling the libiginition libaries using  
`sudo apt-get --reinstall install libignition-math* libignition-fuel-tools*`
