# Gate module type

The Gate module allows to translate Json to Luos and Luos to Json constantly. This module continuously pulls data from the sensors detected on the network and streams it into a Json format. Also, it can receive Json data and convert it into a module command.

You need to have at least one of these modules in one of your nodes to use the Luos network with a computer using Pyluos or any other lib.

Json is a really mainstream standard allowing you to use your favorite language easily trough a Json library.

Its type has access to all common capabilities.

----

## Functions

| **Function name and parameters** | **Action** | **Comment** |
|:---:|:---:|:---:|
| control(self) | Displays module type graphical interface | Only available using Jupyter notebook |

## Variables

| **Variable name** | **Action** | **Type** |
|:---:|:---:|:---:|
| delay | Sets or reads the network refresh delay in ms. | read / write: Integer |

## ROS topics

The gate has no topic but all topics names of all modules are prefixed with the name given to the broker associated to this gate at runtime.
Default is `luos_broker` but can be changed by passing an argument to the launchfile, e.g.: `ros2 launch luos_interface broker.launch.py name:=luos_broker_2`. This name must be unique to prevent conflicts.

<div class="cust_edit_page"><a href="https://{{gh_path}}{{modules_path}}/gate.md">Edit this page</a></div>
