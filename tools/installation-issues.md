# Installation issues

Please install RV2 with the latest version of the dashboard 0.7.1 which can be downloaded here:

[https://github.com/compas-dev/compas\_dashboard/releases](https://github.com/compas-dev/compas\_dashboard/releases)

### 0) Try the normal installation

Install RV2 through the dashboard as you did for IGS by clicking in Install for the RV2 plug-in as shown below:

![](<../.gitbook/assets/image (28).png>)

Now, open Rhinoceros and load the toolbar as in the general tutorial [here](compas-tools.md) and to initialise the plug-in. If you see the screen below it means that everything works and you are ready to used RV2.

![](<../.gitbook/assets/image (293).png>)

If you receive the error: `Unknown command: -RV2_init` type the command `EditPythonScript` and close the window that appears and try to initialise again.

**Only if you still run into problems** follow the **3 steps below** to restart your Environment and install all the plugins from scratch:

### 1) Delete your Environment through the Dashboard

Go to the environment tab in the COMPAS Dashboard as shown below:

![](<../.gitbook/assets/image (47).png>)

Delete the environment by clicking in the red button.

![](<../.gitbook/assets/image (17).png>)

### 2) Clear the plug-ins previously installed in your machine

After you delete the environment on the Rhino Section click the **refresh** button to update the list of plug-ins installed in Rhino as shown below:

![](<../.gitbook/assets/image (13).png>)

Once you refresh the list of Rhino plug-ins you should see the following path where the plug-ins are installed in your computed. The path should look like:

* `C:\Users\YOUR_USER_NAME\AppData\Roaming\McNeel\Rhinoceros\7.0\Plug-ins\PythonPlugins`

The figure below shows how to obtain this path direct from the dashboard:

![](<../.gitbook/assets/image (41).png>)

Open this folder and **delete everything** inside. The folder should be empty:

![](<../.gitbook/assets/image (108).png>)

![](<../.gitbook/assets/image (155).png>)

In addition, also delete all folders in `C:\ ... \AppData\Roaming\McNeel\Rhinoceros\7.0\scripts`.

![](../.gitbook/assets/scripts\_folder.jpg)

Now **CLOSE** and **OPEN** the **Dashboard** and repeat the normal installation.

### 3) Repeat the normal installation

Now that all plug-ins are deleted from the memory, we will open the **Apps** again an repeat the installation:

![](<../.gitbook/assets/image (383).png>)

Click on the install button for RV2:

![](<../.gitbook/assets/image (256).png>)

The installation should work normally now. You can load the toolbar as shown [here](compas-tools.md) and initialise the plug-in seeing the screen below:

![](<../.gitbook/assets/image (400).png>)

Note that If you receive the error: `Unknown command: -RV2_init` you have to type the command `EditPythonScript` and close the window that appears and try to initialise again.

Now you are ready to go to the tutorial.
