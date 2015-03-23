# GEC22 Demonstration March 2015

This demonstration shows the use of Labwiki to plan, prepare, execute and
monitor a research experiment. This experiment will involve a large number of
resources from GENI aggregates in the US and the iMinds aggregate in Europe.

----

## 1. The Experiment

A researcher has designed a 'follow-the-Sun' Content/Service delivery approach,
where contents and services are always provided by datacentres located in a
region with current daylight. These datacentres could be then solar powered.
The researcher's algorithm may also cater for many other optmisation criteria,
such as different renewable power source (e.g. wind turbine, tidal wave, etc...)
or different constraints (e.g. cost).

This experiment is one of the many experiments she could run to evaluate
her new algorithm which dynamically decides which datacentre to redirect a new
client request to.

The initial back-of-the-envelop sketch for that experiment is illustrated below.

<img src="https://raw.githubusercontent.com/mytestbed/gec_demos_tutorial/master/gec22_demo/exp_idea.png" style="width: 70%;" />

The 3-step orchestration of that experiment is further detailed below.

+ Step 1:
    + it is daytime in the geographic region #1
    + many clients from region #1 and a few client from region #2 request some DASH videos
    + the redirection algorithm directs them to a datacentre located in region #1

<img src="https://raw.githubusercontent.com/mytestbed/gec_demos_tutorial/master/gec22_demo/exp_step1.png" style="width: 70%;" />

+ Step 2:
    + it is now daytime in the geographic region #2
    + many clients from region #2 and a few client from region #1 request some DASH videos
    + the redirection algorithm directs them to a datacentre located in region #2

<img src="https://raw.githubusercontent.com/mytestbed/gec_demos_tutorial/master/gec22_demo/exp_step2.png" style="width: 70%;" />

+ Step 3 is a repeat of step 1

<img src="https://raw.githubusercontent.com/mytestbed/gec_demos_tutorial/master/gec22_demo/exp_step3.png" style="width: 70%;" />


## 2. Preparing with LabWiki


In LabWiki, the **Prepare** panel allows you to create, edit and view your experiment
description, which is written using the [OEDL language.](http://mytestbed.net/projects/omf6/wiki/OEDLOMF6)


To **create** a new experiment description, click on the "+" sign, enter a new
filename, select "OEDL", and click on the "Create" button.

![](https://raw.githubusercontent.com/mytestbed/labwiki/master/doc/quickstart/lw_prepare2.png)

To **view** and **edit** an experiment description, type its name in the search
field, for example the simple experiment `demo.oedl`.

![](https://raw.githubusercontent.com/mytestbed/labwiki/master/doc/quickstart/lw_prepare3.png)

After editing your experiment, do not forget to save it by clicking on the disk
icon.

![](https://raw.githubusercontent.com/mytestbed/labwiki/master/doc/quickstart/lw_prepare4.png)


----

## 3. Execute your experiment

In the **Execute** panel, you configure and run your experiment, as well as
view its progress and any defined graphs.

![](https://raw.githubusercontent.com/mytestbed/labwiki/master/doc/quickstart/lw_execute.png)

First, load an experiment description in the **Prepare** panel. For
example, load the `demo.oedl`, then drag and drop the pen-and-paper icon
from the **Prepare** to the **Execute** panel.

![](https://raw.githubusercontent.com/mytestbed/labwiki/master/doc/quickstart/lw_execute2.png)

You can now **configure** the parameters of your experiment, and press the Start
button to **run** the experiment!

![](https://raw.githubusercontent.com/mytestbed/labwiki/master/doc/quickstart/lw_execute3.png)

----

## 4. Observe and analyse

While the experiment is running you can view its properties, any defined graph,
and any message it produces.

![](https://raw.githubusercontent.com/mytestbed/labwiki/master/doc/quickstart/lw_execute4.png)


