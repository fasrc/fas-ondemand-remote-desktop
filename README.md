# Batch Connect - Desktop

A Batch Connect app designed to launch a GUI desktop within a batch job.

## Prerequisites

This Batch Connect app runs a remote desktop session on a compute node from a singularity container 
with the Xfce Desktop

The following nees to be installed on the compute nodes:

For VNC server support:

- [TurboVNC] 2.1+
- [websockify] 0.8.0+

## Install

The master branch of this repository is used as template to generate customized version of the app for different academic courses on FAS-OnDemand.
The actual apps deployed on the cluster are stored in [this repository](https://github.com/fasrc/fas-ondemand-remote-desktop-apps).

If you want to deploy this repo in your user development environment to make modifications, follow these instructions. 

```sh
# create the development folder if you still not have one
mkdir -pv $HOME/.fasrc/dev/
cd $HOME/.fasrc/dev/

# clone the repository in a subfolder for your version of the app
git clone https://github.com/fasrc/fas-ondemand-remote-desktop.git

# Change the working directory to this new directory
cd fas-ondemand-remote-desktop
```
You can now make your preferred modifications and run your version of the app from the sandbox control panel under the
*dev* menu on the ondemand dashboard

## Contributing

If you intend deploy your modified version as system wide app, please commit your changes to a branch first, and open a PR.
