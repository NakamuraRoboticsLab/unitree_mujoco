# H1 Python with IK based on Pinocchio

Unitree H1 gravity compensation control based on Pinocchio. 

Build virtual environment based MiniConda3: 
```bash
mkdir -p ~/miniconda3
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda3/miniconda.sh
bash ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
rm ~/miniconda3/miniconda.sh
```

After installation of MiniConda3, initialize by
```bash
~/miniconda3/bin/conda init --all
source ~/.bashrc
```

Create virtual environment
```bash
conda create -n unitree_py python=3.10 # here unitree_py can be replaced by other name you want
```

Activate virtual environment
```bash
conda activate unitree_py
```

Also need to install unitree_sdk2_python in this environment:
https://github.com/unitreerobotics/unitree_sdk2_python.git


Requirement (in the virtual environment): 
```bash
# Required lib
pip install -r requirements.txt
```

The program will automatically open a webpage for kinematics simulation. 