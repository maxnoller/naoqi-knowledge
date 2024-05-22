# Getting Started

This guide will help you get started with working with Aldebaran robots using the QI library in Python.

## Installing the QI Library

### Using pip

To install the QI library using pip, open your terminal and run the following command:

```sh
pip install qi
```

### Using Poetry

To install the QI library using Poetry, open your terminal and run the following commands:

1. Navigate to your project directory:

```sh
cd your-project-directory
```

2. Add the QI library as a dependency:

```sh
poetry add qi
```

## Finding Out Your Robot's IP Address

To connect to your Aldebaran robot, you need to know its IP address. You can find this information using the following steps:

1. Turn on your robot.
2. Wait for it to fully boot up.
3. Press the robot's chest button. The robot will announce its IP address.

Alternatively, you can use the robot's interface or the Aldebaran software to find the IP address.

## No Robot? Use the Simulator

If you do not have access to a real robot, you can use the simulator provided by Aldebaran. For detailed instructions on setting up and using the simulator, please refer to the [Simulation README](link_to_simulation_readme.md).

## Basic Python Code Example

Here is a basic Python code example that creates a QI session, connects to the Text-To-Speech (TTS) service of NAO, and lets him say "Hello, world":

```python
import qi

def main():
    # Replace '192.168.1.1' with your robot's IP address
    robot_ip = "192.168.1.1"
    robot_port = 9559

    # Create a QI session
    session = qi.Session()

    # Connect to the robot
    session.connect(f"tcp://{robot_ip}:{robot_port}")
    print("Connected to the robot at {}:{}".format(robot_ip, robot_port))

    # Get the TTS service
    tts = session.service("ALTextToSpeech")

    # Make the robot say "Hello, world"
    tts.say("Hello, world")

if __name__ == "__main__":
    main()
```

This script connects to the robot using its IP address and port number, then uses the Text-To-Speech service to make the robot speak.

---

With these steps, you should be ready to start developing with Aldebaran robots using the QI library. If you have any questions or run into issues, feel free to create an issue in the repository.
