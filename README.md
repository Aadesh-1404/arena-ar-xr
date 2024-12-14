# ARENA AR VR Interaction

Mixed Reality interaction between AR and VR users
Any room can be scanned and added to the arena scene. Run the scripts below for interaction.

* [ARENA](arenaxr.org)

### Step 1
Scan the room and store the scan mesh in quest.

### Step 2
Generated 3d objects with one of the two methods below
* [Gaussian Splatting](https://github.com/graphdeco-inria/gaussian-splatting)
-- Take around 300 photos
-- Ran convert.py to get point clouds
-- Ran train.py to generate splat
-- Ran Gaussian Splatting on Touriga GPU
* [3D App Lidar](https://3dscannerapp.com/)

### Step 3
Add objects to the arena in one of the scenes. There is also a script (arena_script.py) that adds objects to the arena scene automatically. 

### Step 4
Run mesh_icp.py to localize the virtual objects with physical objects. We also need to git clone arena-py and have three mesh files in the examples folder to solve dependencies.

### Step 5
Run tools/interaction_button.py to include different buttons, displays, and ways of interactions. 

Multiple users can interact and solve problems, and place objects (like furniture)!! 

