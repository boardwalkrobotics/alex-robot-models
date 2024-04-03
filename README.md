# Alex Robot URDF

This repository contains the Unified Robot Description Format (URDF) files for Alex, a bimanual humanoid robot designed for both research and commercial applications. The URDF Files have been tested in Drake and IHMC's Simulation Construction Set. If you have any trouble loading the URDF please create an issue or contact us and we can work to fix any issues.  

## Overview

The URDF files define the kinematics, inertia data, joints, sensors, etc.

## Usage: Drake

The meshes in the URDF file are referenced with respect to the `alex_description` package, which needs to be added to the package map before importing the model-

```python
parser.package_map().Add(package_name="alex_description", package_path="alex-robot-models/alex_description")

alex_instance = parser.AddModels(file_name="alex-robot-models/alex_description/urdf/20240109_Alex_noHands.urdf")
```

## License

This work is licensed under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](http://creativecommons.org/licenses/by-nc-nd/4.0/).


