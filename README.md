<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/MarkProminic/simple-tasks-provisioner/">
    <img src="https://startcloud.com/assets/logo-big.jpg" alt="Logo" width="200" height="100">
  </a>

  <h3 align="center">Domino Vagrant Build</h3>

  <p align="center">
    An README to jumpstart your build of the Domino Development
    <br />
    <a href="https://github.com/MarkProminic/simple-tasks-provisioner/"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/MarkProminic/simple-tasks-provisioner/">View Demo</a>
    ·
    <a href="https://github.com/MarkProminic/simple-tasks-provisioner/issues">Report Bug</a>
    ·
    <a href="https://github.com/MarkProminic/simple-tasks-provisioner/issues">Request Feature</a>
  </p>
</p>

<!-- TABLE OF CONTENTS -->
## Table of Contents

* [About the Project](#dominovagrant)
  * [Built With](#built-with)
* [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
  * [Installation](#installation)
    * [Mac OS X](https://github.com/MarkProminic/simple-tasks-provisioner/blob/master/MacMojaveReadme.md) -- Quick Start
    * [Windows](https://github.com/MarkProminic/simple-tasks-provisioner/blob/master/Win10ReadMe.md) -- Quick Start
* [Deployment](#deployment)
  * [Cloning](#cloning-the-repo-locally)
  * [Overview](#configuring-the-environment)
  * [Variables](#commonly-changed-parameters)
  * [Source Files](#source-files)
* [Initialization](#starting-the-vm)
  * [Access Methods](#accessing-the-domino-server)
    * [Web](#web-interface)
    * [Notes Client](#access-from-notes-client)
    * [Console](#domino-console)
* [Common Issues](#common-problems)
* [Roadmap](#roadmap)
* [Contributing](#contributing)
* [License](#license)
* [Contact](#authors)
* [Acknowledgements](#acknowledgments)


## DominoVagrant
Primary goal is to use Vagrant and various provisioners to configure a Virtualbox or Bhyve VM.

* **Template:** [Packer](https://app.vagrantup.com/STARTcloud/boxes/debian12-server)
* **Build Source:** [Repo](Notyetavailableforpublicconsumption)

Each Release will be a at the time, stable branch. Recommended to use the latest.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes, as well as what will power the build process of the VMs at Prominic.NET.

### Prerequisites

You will need some software on your PC or Mac:

```
git
Vagrant
Virtualbox
```

## [Dependency Installation](https://github.com/MarkProminic/simple-tasks-provisioner/wiki/Dependency-Installation)


## [Clone, Config and Deploy](https://github.com/MarkProminic/simple-tasks-provisioner/wiki/Clone-and-Deploy)


## Starting the VM

The installation process is estimated to take about 15 - 30 Minutes.

```
vagrant up
```

At this point, you can execute 'vagrant up' in the git checkout directory
to spin up a vm instance, or use the utility scripts
./scripts/vagrant_up.sh, ./scripts/vagrant_up.ps1 to create a log file with the initialization
output in addition to showing on the screen.

Once the system has been provisioned, you can use 'vagrant ssh' to access
it, or again the utility scripts vagrant_ssh.sh/vagrant_ssh.ps1 to create
a log file of the ssh session.

View the contents of the CommandHelp.text for more details.
This file will also be displayed followed each vagrant up operation for
your continued reference.

## The Process
![Provisioning Process](images/vagrant-build-flow.gif)

## Common Problems

### Error for Headless VirtualBox

If you get an error indicating that VirtualBox could not start in headless mode, open Vagrantfile and uncomment this line

```
     #vb.gui = true
```

## Roadmap

See the [open issues](https://github.com/MarkProminic/simple-tasks-provisioner/issues) for a list of proposed features (and known issues).

## Built With
* [Vagrant](https://www.vagrantup.com/) - Portable Development Environment Suite.
* [VirtualBox](https://www.virtualbox.org/wiki/Downloads) - Hypervisor.
* [Ansible](https://www.ansible.com/) - Virtual Manchine Automation Management.

## Contributing

Please read [CONTRIBUTING.md](https://www.prominic.net) for details on our code of conduct, and the process for submitting pull requests to us.

## Authors
* **Joel Anderson** - *Initial work* - [JoelProminic](https://github.com/JoelProminic)
* **Justin Hill** - *Initial work* - [JustinProminic](https://github.com/JustinProminic)
* **Mark Gilbert** - *Refactor* - [MarkProminic](https://github.com/MarkProminic)

See also the list of [contributors](https://github.com/MarkProminic/simple-tasks-provisioner/graphs/contributors) who participated in this project.

## License

This project is licensed under the SSLP v3 License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
