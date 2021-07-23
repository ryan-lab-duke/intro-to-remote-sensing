# GEOG 485/585 Remote Sensing I (Fall 2021)

Geog 4/585 is an introduction to remote sensing - the acquisition of data about the world from afar. Often this is in the form of digital imagery acquired by aircraft or satellites, but a variety of other types of remote sensing exist and are discussed in the class.

The course provides an overview of the physical science principles involved in remote sensing, the instruments and platforms used to collect data, and the analysis/visualization of the acquired information. Topics include data acquisition and pre-processing, image enhancement,  data classification and visualization. The emphasis of the class is on pixel-based raster spectral data (such as satellite or drone imagery), and other types of remote sensing information - such as lidar, radar, and structure-from-motion (SfM) are also addressed in lectures and lab exercises.

## Instructors and Office Hours

**Instructor:** Johnny Ryan (Assistant Professor) |  jryan4@uoregon.edu

**Office Hours:**  Wednesdays 11 tp 11:50am and 1:30 to 2:45pm

Sign up for individual 15 minute time slots via ...
If meeting times are full, or these weekly time periods do not work for you, please email Johnny for a different appointment time.

**GE/Lab Instructor:** XXX XXX (xxx@uoregon.edu)
**Office Hours:** Tuesdays 10:00 - 11:30 am

## Syllabus

The syllabus can be downloaded [here](https://github.com/JohnnyRyan1/intro-to-remote-sensing/blob/master/syllabus/Syllabus.doc).

## Overview of weekly assignments

### Week 1

* [Short lecture assignment](https://github.com/JohnnyRyan1/intro-to-remote-sensing/blob/master/assignments/week_1/remote_sensing_questions.txt)
* [Lab 1 - Remote Sensing Data](https://github.com/JohnnyRyan1/intro-to-remote-sensing/blob/master/assignments/week_1/lab.txt)

### Week 2

## Run the lecture notes interactively ##

The best way to get the materials (including homework) is the use [git](https://git-scm.com/) to [clone this repository](https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository). If you don't have git already on you computer, it is easy to install on all platforms following [these instructions](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).

From the command line, run the command

```bash
git clone https://github.com/rabernat/intro_to_physical_oceanography
```

If you are not a fan of the command line, there are plent of [graphical interfaces to git](https://git-scm.com/download/gui/linux) available.

Once you have the repository cloned, you can update it as new lectures come out by running

```bash
git pull origin master
```

If for some reason you can't get git working, the alternative is to use the link to the right to "Download Zip". The disadvantage here is that you will have to re-download every time the repo is updated.

In order to actually execute the code in the notebooks, you need to have the necessary python packages installed.
The recommended way to do this is to install the [anaconda python distribution](https://www.anaconda.com/download/) together with the [conda package management utility](https://conda.io/docs/).
For more depth, you can read my [detailed intstructions for installing python](https://rabernat.github.io/research_computing/python.html).

This repository includes an [environment file](https://github.com/rabernat/intro_to_physical_oceanography/blob/master/phys_ocean_env.yml) which you can use to set up your python environment. To install this environment, type the following

```bash
cd intro_to_physical_oceanography
conda env create -f phys_ocean_env.yml
```

This will create a new environment called `phys_ocean`. To activate this environment, type

```bash
source activate phys_ocean
```

The notebooks can be viewed and run using the [jupyter notebook](https://jupyter-notebook.readthedocs.io/en/stable/notebook.html) application. To launch the notebook interface, just type

```bash
jupyter notebook
```

When you are done working with the notebooks, close the notebook app and, if you wish, deactive the environment by typing

```bash
source deactivate
```

## Why Python ##

A great deal has been written on [this subject](http://cyrille.rossant.net/why-using-python-for-scientific-computing/).
My reasons are summarized as follows.

1. __Python is open source__. [Open source](https://en.wikipedia.org/wiki/Open_source)
means that the source code is available freely to the public and can be examined,
modified, and improved. The alternative to open source is closed, proprietary.
Proprietary tools, such as MATLAB, are ultimately controlled by corporations, and
those corporations decide what features they will include. I consider software
tools as a central part of scientific research---if we want to have transparent,
reproducible, scientific results, we should be using open source tools.
[Nature](http://www.nature.com/nature/journal/v482/n7386/full/nature10836.html)
agrees with me.

1. __Python is free__. It does not cost money to use python. If your scientific
code is written in MATLAB, it can only be run by others with access to MATLAB.
That means people outside the university world (e.g. high school students), in
economically disadvantaged communities, or in developing countries will be
unable to reproduce and build on your results.

1. __Python is easy to read__. This may seem like a superficial point, but it is
crucial for effective sharing of code. Even if you are the only one reading
your code, python is easy on the eyes.

1. __Python has a great library__. The [scipy ecosystem](http://scipy.org)
provides the tools to do almost anything you can imagine.

1. __Python is constantly evolving__. If you find something you _can't_ do with
python, chances are someone is working on it. The world is changing: data is
exploding, computers architecture is evolving, and new forms of analysis and
visualization are being invented. Python is evolving too, and it evolves based
on what the community needs. The new tool I am most excited about is
[xray](http://continuum.io/blog/xray-dask).

1. __Python is at home on the web__. The [Jupyter project](https://jupyter.org/)
grew out of the python community and is revolutionizing the way we do science
and communicate it with others. With Jupyter, I never have to leave my browser.
[Nature agrees](http://www.nature.com/news/interactive-notebooks-sharing-the-code-1.16261)
that this is the future of scientific communication.
