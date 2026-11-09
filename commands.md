1) PREPARE GIT
git config user.name "AlexMed"
git config user.email "workEmail@company.com"

2) 
## LAUNCH IT
### macOS
python3 -m venv .venv
source .venv/bin/activate
python3 calibrate_camera.py

### Power shell
python3 -m venv .venv
Set-ExecutionPolicy -Scope CurrentUser
  tell: RemoteSigned
.venv\Scripts\Activate.ps1
pip install git+https://github.com/AlexanderAMedvedev/SOME_DEPENDENCY.git@SOME_TAG
  (opencv-python и numpy ставятся вместе с cv_shared как его зависимости)
   # in other cases
     pip install opencv-python
.venv\Scripts\python.exe calibrate_camera.py

3) install all dependencies from the *.toml - file for the current project
pip install . && pip uninstall -y <your-project> 

