# IV and V - COMPAS plugins

This tutorial will cover the installation of the **COMPAS** plugins necessary to this course which will be installed in three main steps.

1. Install **Anaconda 3**, a library of open-source python packages
2. Install the **COMPAS Dashboard** which allows getting access to the latest versions of the plug-ins.
3. Get the plugin (IGS, RV2, PGS) of the respective class set up in Rhinoceros.

{% hint style="info" %}
If you are sure you already have Anaconda installed in your computed you can skip the first step.
{% endhint %}

## 1. Installing Anaconda 3

### 1.1. Get the installer

The Installation of Anaconda can be done through the link below. The installtion is free and **do not require any** registration. Note the installer download starts once you click in the `Download` button in green.

* [https://www.anaconda.com/products/individual](https://www.anaconda.com/products/individual)

![](<../.gitbook/assets/image (26).png>)

### 1.2. Open the installer

Open the installer and follow the default instructions. The program should be installed in the default location `C://Username/anaconda3/` unless you receive an error, forthese cases see the troubleshooting below.

![](<../.gitbook/assets/image (31).png>)

Follow all the default installations and you got Anaconda in your machine! You can go to the step 2 of this tutorial. In case you ran into any trouble please se the section below.

### 1.3. Troubleshooting for usernames with spaces  '\_'

If your username contain white spaces `' '` or special caracteres `éáã'ç` you will see the following warning that **should not be ignored**. Multiple python packages have trouble running into usernames with spaces. To avoid that we will install Anaconda in a different location.

![](<../.gitbook/assets/image (365).png>)

If you saw that warning please create a folder named `anaconda3` within your local drive `C:\` the final adresss should look like in the following image. After that please accept all the default settings.

![](<../.gitbook/assets/image (64).png>)

You are good to go to step 2.

## 2. Installing COMPAS Dashboard

### 2.1. Get the dashboard

The COMPAS dashboard makes it easy to get always the latest version of the COMPAS plug-ins that will be used in the course. Please download the latest version of the Dashboard available in the following link. (What you need is the .exe file)

* [https://github.com/compas-dev/compas\_dashboard/releases](https://github.com/compas-dev/compas\_dashboard/releases)

![](<../.gitbook/assets/image (105).png>)

### 2.2. Install and open the Dashboard

Open the dashboard. Please note that the file will be protected after you download and might be blocked by your browser. Please click to keep it or accept it so you can get continue the installation. If everything goes as expected you should see the dashboard like in the figure below, and you can move to the step 3.

![](<../.gitbook/assets/image (262).png>)

If you had to change the original location of Anaconda (Section 1.3) you will see an error in the dashboard, in this case please procede to section 2.3.&#x20;

### 2.3. Troubleshooting in case Anaconda location is not found

If by any reason you installed Anaconda in a different location in your computer you need to let the Dashboard know where this location is. The image below shows how to do that. The correct location should be: `C:\anaconda3\` (see 1.3).

![](<../.gitbook/assets/image (74).png>)

## 3. Get the plug-in for the class

### 3.1. Prepare Rhino to install Python plug-ins

Open a Rhino windows and type at least once the command `EditPythonScript` you will see a window pop up. You can **close this window** and **close Rhino** as well. This is required to initialise a few folders in your computer and does not have do be done if you already used Python Scripting in Rhino.

![](<../.gitbook/assets/image (42).png>)

Now, refer back to the Dashboard to install the desired plug-in.

### 3.2. Install desired plug-in

Once you have the dashboard working scroll down on the dashboard and press `COMPAS APPS`

You should see the three apps that will be used in the course. Check for the **latest** **version** of the **plug-in** desired, select the **appropriate Rhino version** and press install.

![](<../.gitbook/assets/image (285).png>)

The installation window will open and you will be asked to accept a few modifications on your computer. Press `Yes` to these and the installation is complete.

![](<../.gitbook/assets/image (339).png>)

### 3.3. Load the plug-in toolbar

At last, open Rhino and in the Menu go to `Tools > ToolbarLayout`

On the Toolbar Layout window go to `File > Open` and load the toolbar of the corresponding plug-in downloaded. The toolbar should already be placed in the Rhino default toolbars location, which is shown in the image below: &#x20;

![](<../.gitbook/assets/image (409).png>)

Press open and the toolbar will load. In the following picture the toolbar for `IGS` is shown:

![](<../.gitbook/assets/image (284).png>)

Different plug-ins can be installed at the same time, and each plugin has its own toolbar. These toolbars can be shown/hidden always accessing the toolbar layout

These plug-ins will now be used for the modules IV, V and VI. :tada:
