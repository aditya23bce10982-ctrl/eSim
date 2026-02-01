# eSim 2.5 Installation Analysis on Ubuntu 25.x

## Tested Environment
- OS: Ubuntu 25.10 (VirtualBox VM)
- Architecture: x86_64
- Python: 3.12.x
- Date: January 2026

## Objective
To identify and document installation and compatibility issues of eSim 2.5 on Ubuntu 25.x systems.

## Issue 0: Missing install-eSim.sh Script
The INSTALL file references install-eSim.sh, but the script is not present in the repository, making installation impossible.

## Issue 1: Unsupported Ubuntu Version
eSim officially supports Ubuntu only up to 24.04. The installer does not validate Ubuntu 25.x.

## Issue 2: Broken INSTALL Instructions
INSTALL references missing scripts and provides no fallback installation steps.

## Issue 3: Python 3.12+ setup.py Failure
Legacy setup.py workflow is incompatible with Python 3.12+.

## Issue 4: Qt Dependency Incompatibility
Required PyQt bindings are unavailable or incompatible on Ubuntu 25.x.

## Issue 5: VirtualBox Disk Space Constraint
APT operations initially failed due to insufficient VM disk allocation.

## Conclusion
eSim 2.5 is currently incompatible with Ubuntu 25.x without significant installer modernization.
