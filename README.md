# -Lab-5_202001413
Static Analysis


IT314 - Software Engineering

Lab 5 - Static Analysis

Name: shubham patel
ID: 202001413

Static Analysis:

To perform the above analysis I have used python files from github repository and used pylint to do static analysis for the files.

Repository that i have used for static analysis:
https://github.com/shubham7013/SE_lab_202001413.git

Pylint 

It’s been around for 13 years, and over that time it has included features like coding standards, error detection and refactoring by detecting duplicated code.

Out of the box Pylint is easy to set up, requiring a minimal amount of configuration, but it’s fully customizable if you want it to be — by editing a file you can select which errors and conventions are most relevant to you.

Most of the messages here will be self-explanatory.

Pylint is an incredibly useful tool for static code analysis. It provides a simple score out of 10, a detailed output on what to fix, and the ability to ignore things you do not believe in.

This is part one of three of a series I am doing on how I use pylint in my projects.
Part 1: Executing with Command Line vs Programmatically
Part 2: Pylint Runner Script with Changeable Threshold
Part 3: A Github Action for Failing Builds under a Pylint Threshold




$ pip install pylint

This should give you confirmation it is installed.

$ pylint src/ or py -m pylint file.py

Which should give you some output from the static code analysis followed by a score!

I have used a repository named qxresearch-event-1-master for stat analysis.

Here above attached is pylint been installed.










Now I will check for 6 different files for stat analysis 
![Screenshot (58)](https://user-images.githubusercontent.com/96972155/225274028-467e28fc-7d3a-4817-9ccf-13a58167cbe1.png)

File 1 -> passpdf
![Screenshot (47)](https://user-images.githubusercontent.com/96972155/225274521-31211af4-4c3b-48d8-af2c-c3f344e51b73.png)

here pylint have given us error 
alarmtiming.py:3:0: C0411: standard import "import winsound" should be placed before "from playsound import playsound" (wrong-import-order)

File 2 -> alarmtiming
![Screenshot (48)](https://user-images.githubusercontent.com/96972155/225274569-a526e1a8-023d-4be4-a638-7010f72e78eb.png)
calendar.py:1:0: W0614: Unused import enum from wildcard import (unused-wildcard-import)
calendar.py:1:0: W0614: Unused import sys from wildcard import (unused-wildcard-import)
calendar.py:1:0: W0614: Unused import types from wildcard import (unused-wildcard-import)
all of the erorr are related to unused-wildcard-import.

File 3 -> calendar
![Screenshot (49)](https://user-images.githubusercontent.com/96972155/225274591-32ce2be6-16c2-4424-befe-ffe40bb228af.png)
![Screenshot (50)](https://user-images.githubusercontent.com/96972155/225274614-c98d14c6-4137-49d9-a44e-388969e3d135.png)

paint.py:1:0: W0614: Unused import sys from wildcard import (unused-wildcard-import)
paint.py:1:0: W0614: Unused import types from wildcard import (unused-wildcard-import)
paint.py:1:0: W0614: Unused import TclError from wildcard import (unused-wildcard-import)
all of the erorr are related to unused-wildcard-import.





File 4 -> paint
![Screenshot (51)](https://user-images.githubusercontent.com/96972155/225274752-c6ad96de-6722-43b3-9a47-bf31ef3644d1.png)
![Screenshot (52)](https://user-images.githubusercontent.com/96972155/225274784-69e89152-ead5-4a95-8b1e-47f1e4a46cc7.png)
![Screenshot (53)](https://user-images.githubusercontent.com/96972155/225274801-f155f19f-a1bd-4f59-aa27-c6865fbdcc72.png)
paint.py:1:0: W0614: Unused import sys from wildcard import (unused-wildcard-import)
paint.py:1:0: W0614: Unused import types from wildcard import (unused-wildcard-import)
paint.py:1:0: W0614: Unused import TclError from wildcard import (unused-wildcard-import)
all of the erorr are related to unused-wildcard-import.




File 5 -> random pass
![Screenshot (54)](https://user-images.githubusercontent.com/96972155/225274845-7cd2a7ba-5ae0-40c0-822a-0f1d7fd8ac59.png)
![Screenshot (55)](https://user-images.githubusercontent.com/96972155/225274876-1ee2ddd9-099f-4ece-b7d1-387384858a1e.png)
![Screenshot (56)](https://user-images.githubusercontent.com/96972155/225274910-f7684bef-e218-4a4c-b269-0636017fc849.png)

this file had much less errors compared to other files I analysed.





File 6 -> source-code
![Screenshot (57)](https://user-images.githubusercontent.com/96972155/225274937-91343fcc-0248-4da1-876e-cc8201784e88.png)

source-code.py:44:0: W0311: Bad indentation. Found 12 spaces, expected 8 (bad-indentation)
source-code.py:1:0: C0103: Module name "source-code" doesn't conform to snake_case naming style (invalid-name)
error related to above 2 bad indentation and invalid name can be resolved easily.





