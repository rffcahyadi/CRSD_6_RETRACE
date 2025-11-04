PART 1: 3D Scanning with Reality Scan Mobile

This is a set of instructions for 3D scanning the artefact.
We used the app Reality Scan Mobile from Epic Games on a smartphone with a LiDAR feature. 

The full documentation can be accessed at this link:

https://dev.epicgames.com/documentation/en-us/realityscan-mobile/realityscan-step-by-step-guide

With the method we used, the steps are:

1. Go to the artefact on a clear day if possible. This will help in making the result more detailed.

2. Clean the area from obstructing objects such as dry leaves, dirt, etc., depending on your needs.

3. Open the Reality Scan Mobile App and use the Augmented Reality mode.

4. Take pictures with the main artefact in the middle of the frame, increasing the number of faces captured by the camera and the overlapping images.

5. Review the scan to see if there are enough images and the point clouds generated are sufficient.

6. Crop/cut the unnecessary part from the scan so it only shows you artefact.

7. Export the mesh file and send it to the computer.



PART 2: ShrinkWrap

PART 3:

This is the script to find the Areas of Interest from your scanned mesh.
It consists of several numbered parts:

0. PARAMETER
This is where you can change the parameter of this script to get the AOIs. You can change them based on the level of detail you want to achieve. Other than that, this is used to adjust the output because it is always different cases for every mesh.

1. EXTERIOR REMOVAL
On this section you can change:
List item: based on which faces you want to exclude



2. CURVATURE DETECTION
On this section you can change:
Contour Distance: higher number, more detailed
Rebuild Curve Count: higher number, more detailed
Curvature Threshold: higher number, more detailed

3. ANGLE DETECTION
On this section you can change:
Angle threshold: based on limitation of extruder (range of motion)

4. HEIGHT DETECTION
On this section you can change:
Height threshold: based on the limitation of extruder (nozzle height)

5. CLUSTERING AOIs
On this section you can change:
X Tolerance: based on how close you want the cluster tolerance to be
Y Tolerance: based on how close you want the cluster tolerance to be

6. REMOVE OVERLAPPING AOIs
On this section you can change:
Box Size: how big you want the AOIs to test print
X Overlapping Tolerance: based on how close you want the cluster tolerance to be
Y Overlapping Tolerance: based on how close you want the cluster tolerance to be

7. MESH AOIs OUTPUT
On this section you can change:
X_False Mesh Removal Index: select the mesh unwanted
X_False Mesh Removal Tolerance: Trial and Error, find the AOIs with closed mesh
Y_False Mesh Removal Index: select the mesh unwanted
Y_False Mesh Removal Tolerance: Trial and Error, find the AOIs with closed mesh







