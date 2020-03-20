[![Github top language](https://img.shields.io/github/languages/top/FHPythonUtils/ImageRound.svg?style=for-the-badge)](../../)
[![Codacy grade](https://img.shields.io/codacy/grade/caca6f53db3a44f08b7cbdb25284e784.svg?style=for-the-badge)](https://www.codacy.com/manual/FHPythonUtils/ImageRound)
[![Codacy coverage](https://img.shields.io/codacy/coverage/caca6f53db3a44f08b7cbdb25284e784.svg?style=for-the-badge)](https://www.codacy.com/manual/FHPythonUtils/ImageRound)
[![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/ImageRound.svg?style=for-the-badge)](../../)
[![Issues](https://img.shields.io/github/issues/FHPythonUtils/ImageRound.svg?style=for-the-badge)](../../issues)
[![License](https://img.shields.io/github/license/FHPythonUtils/ImageRound.svg?style=for-the-badge)](/LICENSE.md)
[![Commit activity](https://img.shields.io/github/commit-activity/m/FHPythonUtils/ImageRound.svg?style=for-the-badge)](../../commits/master)
[![Last commit](https://img.shields.io/github/last-commit/FHPythonUtils/ImageRound.svg?style=for-the-badge)](../../commits/master)
[![PyPI Downloads](https://img.shields.io/pypi/dm/imageedit.svg?style=for-the-badge)](https://pypi.org/project/imageedit/)
[![PyPI Version](https://img.shields.io/pypi/v/imageedit.svg?style=for-the-badge)](https://pypi.org/project/imageedit/)

<!-- omit in toc -->
# ImageEdit

<img src="readme-assets/icons/name.png" alt="Project Icon" width="750">

[**Now available on pypi.org!**](https://pypi.org/project/imageedit/)

Create various icon masks and shading effects with the imageedit library.
Four example files: round.py, makeProjIcons.py, makePWAImages.py and
getPWAScreenshots.py. Includes imagetracer.py. imagetracer.py uses JS and is
much faster than previous implementations. Takes a few seconds and has no cap.

- [Library Files](#library-files)
- [Example Files](#example-files)
- [Comparison to similar solutions](#comparison-to-similar-solutions)
	- [GUI](#gui)
	- [Web](#web)
	- [Advantages of this solution](#advantages-of-this-solution)
	- [Disadvantages of this solution](#disadvantages-of-this-solution)
- [How to use out of the box (makePWAImages)](#how-to-use-out-of-the-box-makepwaimages)
- [Install With PIP](#install-with-pip)
- [Language information](#language-information)
	- [Built for](#built-for)
- [Install Python on Windows](#install-python-on-windows)
	- [Chocolatey](#chocolatey)
	- [Download](#download)
- [Install Python on Linux](#install-python-on-linux)
	- [Apt](#apt)
- [How to run](#how-to-run)
	- [With VSCode](#with-vscode)
	- [From the Terminal](#from-the-terminal)
- [Changelog](#changelog)
- [Download](#download-1)
	- [Clone](#clone)
		- [Using The Command Line](#using-the-command-line)
		- [Using GitHub Desktop](#using-github-desktop)
	- [Download Zip File](#download-zip-file)
- [Licence](#licence)
- [Screenshots](#screenshots)
	- [Desktop](#desktop)

## Library Files
See the [Docs](/Docs.md) for more information.
## Example Files
- round.py
- makeProjIcons.py
- makePWAImages.py
- getPWAScreenshots.py

## Comparison to similar solutions

Similar solutions include but are not limited to:

### GUI
https://www.getpaint.net/

### Web
https://realfavicongenerator.net/

### Advantages of this solution
- Minimal: few dependencies required (python and pillow)
- Quick: when given a regular or mask image it can produce a large number or
variants in a relatively short amount of time
- Customisable: write your own scripts to leverage imageEdit (python knowledge
required)
- Produce a PWA mask icon out of the box
- SVG tracing lib doesn't require potrace/ pypotrace which can be challenging to
set up on Windows
- SVG tracing using imageTracerJs.py (https://github.com/jankovicsandras/imagetracerjs)
is pretty good (requires pyppeteer: https://github.com/miyakogi/pyppeteer)

### Disadvantages of this solution
- Specific image dimensions needed out of the box: whilst this is something that
could be changed, maskable icons are 640x640 and regular icons are 512x512

## How to use out of the box (makePWAImages)

1. Put regular 512x512 image or mask 640x640 image under main/input in this
example I am using lightfox.png

<img src="readme-assets/examples/lightfox.png" alt="LightFox" width="128">

2. Run ```makePWAImages.py``` and navigate to main/output/lightfox.png/pwa

<div>
<img src="readme-assets/examples/mask.png" alt="LightFox" width="128">
<img src="readme-assets/examples/round-192.png" alt="LightFox" width="38">
<img src="readme-assets/examples/round-512.png" alt="LightFox" width="102">
<img src="readme-assets/examples/square-180.png" alt="LightFox" width="36">
<img src="readme-assets/examples/squircle-256.png" alt="LightFox" width="52">
</div>

## Install With PIP

```python
pip install imageedit
```

Head to https://pypi.org/project/imageedit/ for more info

See python files under main for example usage

## Language information
### Built for
This program has been written for Python 3 and has been tested with
Python version 3.8.0 <https://www.python.org/downloads/release/python-380/>.

## Install Python on Windows
### Chocolatey
```powershell
choco install python
```
### Download
To install Python, go to <https://www.python.org/> and download the latest
version.

## Install Python on Linux
### Apt
```bash
sudo apt install python3.8
```

## How to run
### With VSCode
1. Open the .py file in vscode
2. Ensure a python 3.8 interpreter is selected (Ctrl+Shift+P > Python:Select
Interpreter > Python 3.8)
3. Run by pressing Ctrl+F5 (if you are prompted to install any modules, accept)
### From the Terminal
```bash
./[file].py
```

## Changelog
See the [CHANGELOG](/CHANGELOG.md) for more information.

## Download
### Clone
#### Using The Command Line
1. Press the Clone or download button in the top right
2. Copy the URL (link)
3. Open the command line and change directory to where you wish to clone to
4. Type 'git clone' followed by URL in step 2
```bash
$ git clone https://github.com/[user-name]/[repository]
```
####

More information can be found at
<https://help.github.com/en/articles/cloning-a-repository>

#### Using GitHub Desktop
1. Press the Clone or download button in the top right
2. Click open in desktop
3. Choose the path for where you want and click Clone

More information can be found at
<https://help.github.com/en/desktop/contributing-to-projects/cloning-a-repository-from-github-to-github-desktop>

### Download Zip File

1. Download this GitHub repository
2. Extract the zip archive
3. Copy/ move to the desired location

## Licence
MIT License
Copyright (c) fredhappyface
(See the [LICENSE](/LICENSE.md) for more information.)

## Screenshots

### Desktop
<div>
<img src="readme-assets/screenshots/desktop/screenshot-0.png" alt="Screenshot 1" width="600">
<img src="readme-assets/screenshots/desktop/screenshot-1.png" alt="Screenshot 2" width="600">
<img src="readme-assets/screenshots/desktop/screenshot-2.png" alt="Screenshot 3" width="600">
</div>
