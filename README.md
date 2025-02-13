# 3Laws Robotics Repository

<br>
<p align="center">
  <a href="https://github.com/3LawsRobotics/3laws">
    <img src="media/logo.png" alt="Logo" width="639" height="301">
  </a>

  <h3 align="center">3Laws Robotics' Public Repo</h3>

  <p align="center">
    <a href="https://github.com/3LawsRobotics/3laws/"><strong>Explore the repo»</strong></a>
    <br />
    <a href="https://3LawsRobotics.github.io/3laws/"><strong>Explore the docs»</strong></a>
    <br />
  </p>
</p>

## Introduction

This repository purpose is to offer an easy access to the binary files of the 3Laws Robotics products.
The first public release of the [**Supervisor**](#Robot-diagnostic-module-installation)
is already available at a beta state. To get more information about this product, please contact [support@3lawsrobotics.com](support@3lawsrobotics.com)

Documentation and Tutorial will soon be available.

## Forum

Issues, questions, announcements and general discussions can be created and found at: [https://github.com/3LawsRobotics/3laws/discussions](https://github.com/3LawsRobotics/3laws/discussions).

## Releases

Release changelog and files can be found at: [https://github.com/3LawsRobotics/3laws/releases](https://github.com/3LawsRobotics/3laws/releases).
This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html), although API compatibility is only guaranteed from version `1.0.0` onward.

## Supervisor installation

### Interactive Package installation

```bash
bash <(curl https://raw.githubusercontent.com/3LawsRobotics/3laws/master/install.sh)
```

### Specific package

You can add arguments after the command to specify the wanted ros and ubuntu version, the desired CPU architecture and non interactive arguments like Always Yes and Force.

- `-a <ARCH [amd64, arm64]>`
- `-v <UBUNTU_DISTRO [18.04, 20.04, 22.04]>`
- `-r <ROS_DISTRO [iron, humble, galactic, foxy, noetic]>`
- `-f <Force even if versions doesn't match>`
- `-y <Always yes>`

```bash
bash <(curl https://raw.githubusercontent.com/3LawsRobotics/3laws/master/install.sh) [-hyf] [-r <ROS_DISTRO>] [-a <ARCH>] [-v <UBUNTU_VERSION>]
```

### Non interactive

Download the package:

```bash
wget https://raw.githubusercontent.com/3LawsRobotics/3laws/master/install.sh
```

Make it executable:

```bash
chmod +x install.sh
```

Run it with your arguments:

```bash
sudo ./install.sh [-hyf] [-r <ROS_DISTRO>] [-a <ARCH>] [-v <UBUNTU_VERSION>]
```

if `-yf -r <ROS_DISTRO> -a <ARCH> -v <UBUNTU_VERSION>` specified, the script is non interactive

As an example:

```bash
sudo ./install.sh -yf -r foxy -a arm64 -v 20.04
```

## Supervisor uninstall:

This command will fully remove supervisor from your computer

```bash
bash <(curl https://raw.githubusercontent.com/3LawsRobotics/3laws/master/uninstall.sh)
```

## Repo maintainer

Thomas Gurriet - tgurriet@3laws.io
