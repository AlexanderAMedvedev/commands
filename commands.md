# PREPARE GIT
git config user.name "AlexMed"
git config user.email "workEmail@company.com"

# PREPARE .ENV FOR PYTHON PROJECT AND RUN THE PROJECT FROM COMMAND LINE
## macOS
python3 -m venv .venv
source .venv/bin/activate

python3 calibrate_camera.py

## Windows
python3 -m venv .venv
Set-ExecutionPolicy -Scope CurrentUser
  `type the answer:` RemoteSigned
.venv\Scripts\Activate.ps1

.venv\Scripts\python.exe calibrate_camera.py

# INSTALL DEPENDENCIES FROM THE *.toml - FILE FOR THE PROJECT
pip install git+https://github.com/AlexanderAMedvedev/SOME_DEPENDENCY.git@SOME_TAG

pip install opencv-python

pip install .
pip uninstall -y <your-project>

pip install uv
uv sync --all-groups
