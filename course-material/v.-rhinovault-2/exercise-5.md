# Exercise

{% hint style="info" %}
Please complete the 4 tasks below, and submit a zipped folder that includes the requested files by **9:00am on Friday, December 3rd**.

Please follow the file naming convention as shown in the [**Syllabus**](../../syllabus.md#submissions). &#x20;

### [Submit exercise 5 here.](https://www.dropbox.com/request/G2gFIQZ6yp0VMhnILmdc)
{% endhint %}

For each of the four tasks below, complete and submit a .rv2 file, as well as the completed PDF for the exercise.

{% file src="../../.gitbook/assets/CSD1_2021_exercise-5_template (1).docx" %}

## Task 1 - Modifying force diagram

In the first task, you will design a shell with a rectangular footprint. Since you will be stretching parts of the force diagram to make creases in the thrust diagram, you will need to consider the appropriate method for generating a topology of the pattern that is structured and easy to control later. The ratio of the two sides of the rectangle should be 5:2. The longer sides will be fully supported, while the shorter sides will remain unsupported. Apply a sag of 10% for the open boundaries.

Once the horizontal and vertical equilibrium have been computed, create 4 creases in the direction perpendicular to the fully supported edges. You are free to place the creases in any area of the shell. For the edges that correspond to the creases, elongate them by the following amounts:&#x20;

* Crease 1: 2 times their current lengths
* Crease 2: 6 times their current lengths
* Crease 3: 3 times their current lengths
* Crease 4: 4 times their current lengths&#x20;

{% hint style="info" %}
For this first task, save the result as `exercise-5_task1_Name.rv2` and submit it together with the completed .pdf template.
{% endhint %}

## Task 2 - Holes

In the second exercise, you will design a free-form shell with openings and holes. Download and use the Rhino file below to start the exercise.

{% file src="../../.gitbook/assets/CSD1_2021_exercise-5_task-2 (1).3dm" %}

#### Step 1 - your name

Every letter of the alphabet has been assigned a random length. For every letter of your name (choose either first or last name, or both if the name(s) are too short!), copy and paste the lines corresponding to the letter, as shown below.

![Figure 1 - Example using the name "Juney"](<../../.gitbook/assets/image (225).png>)

#### Step 2 - boundary

In the Rhino file provided, you should see three concentric circles below the alphabet and the letters. Using the Rhino command `ArrayPolar`, generate a polar array of lines with the same number of letters for the name that you used in the previous step. Adjust each of the lines accordingly, then connect the endpoints of these lines using the `Polyline` command. This polyline will be the outer boundary of the shell (Figure 2a).

#### Step 3 - holes

Add two circular holes, each with a different radius, inside the boundary (Figure 2b). Using `Create Pattern` > `FromTriangulation`, generate a triangulated pattern from the outer boundary (polyline) and the inner boundaries (the two circles) using a target edge length you think is reasonable for the size and the configuration of the boundaries (Figure 2c).&#x20;

#### Step 4 - Boundary conditions

Initially, only the corner vertices of the outer boundary will be used as supports (the two circular inner boundaries will become holes of the shell, not supports). By using `Define Boundary Conditions` > `UpdateBoundaries` command, assign an appropriate amount of sags to each of the open boundaries.&#x20;

{% hint style="danger" %}
As a design constraint, the client requests that the holes remain circular in plan!

**Hint**: Any vertices can be assigned or unassigned as supports at any time.
{% endhint %}

![Figure 2 - a) polyline connecting the endpoints of the lines with lengths corresponding to the letters of the name; b) add two holes; c) pattern from triangulation; d) adjust boundary openings.](../../.gitbook/assets/exercise-5\_task-2.jpg)

#### Step 5 - Inner supports

After horizontal and vertical equilibrium have been computed, select a few vertices along the larger circular opening, and create a dropdown similar to the one in the Armadillo Vault (Figure 3).

![Figure 3 - The central dropdown of the Armadillo Vault.](<../../.gitbook/assets/image (151).png>)

{% hint style="info" %}
For this task, save the result as `exercise-5_task2_Name.rv2` and submit it together with the completed .pdf template.
{% endhint %}

## Task 3 - Touchdowns + smoothing

#### Part A - Pattern

For this task, you are asked to cover a courtyard with a circular support in the middle with a shell roof structure, similar to the Great Court of the British Museum (Figure 4).

![Figure 4 - The Great Court of the British Museum.](<../../.gitbook/assets/image (362).png>)

The site has a rectangular outer boundary at level 15, and a circular inner boundary at level 10. All the supports on the outer boundary must lie on the rectangle that is 15 meters above the ground, and all the supports on the inner boundary must lie on the circle that is 10 meters above the ground (Figure 5).

In addition, the client has requested that additional vertical supports are placed around the circular inner boundary, such that the spacing between any two columns, or between any column and the boundaries is no more than 10 meters.

![Figure 5](<../../.gitbook/assets/image (125).png>)

By using `Create Pattern` > `FromFeatures` command, create a quad mesh from the two boundaries (shown in red). Vertically move the supports accordingly so that all the supports on the outer boundary lie on the rectangle at level 15, and all the supports on the inner boundary lie on the circle at level 10. To create these additional supports, either:

* Use points as additional inputs during the decomposition of the pattern generation, to create the singularities where the columns will be placed.
* Change the vertex of the ThrustDiagram into a support.

You are free to choose the height of the column (you can vertically move the singularity down to any elevation).&#x20;

As a last request, the client asks you to make the surface of the shell as smooth as possible. Use the appropriate `Modify _____ Diagram` commands to smoothen the surface of the shell.

{% hint style="danger" %}
**Hint**: A smoother surface of the shell means the force distribution is more consistent and even throughout.
{% endhint %}

Download and use the Rhino file below to start the exercise.

{% file src="../../.gitbook/assets/CSD1_2021_exercise-5_task-3.3dm" %}

{% hint style="info" %}
For this task, save the result as `exercise-5_task3_Name.rv2` and submit it together with the completed .pdf template.
{% endhint %}

## Task 4 - Free design

Pick the first letter of your name or last name and design a shell inspired by the shape of the letter using the command "Create pattern from Skeleton" (Fig.6). You are free to add features and customise your shell. As a mandatory requirement, the shell must be in horizontal and vertical equilibrium.

![Shell with the shape of the letter A, created using "create pattern from skeleton".](<../../.gitbook/assets/image (322).png>)

{% hint style="info" %}
For this fourth task, save the result as `exercise-5_task4_Name.rv2` and submit together with the completed .pdf template.
{% endhint %}
