# C2P2sem2025-PythonExercises
To set-up the columnar analysis exercises, we need to be able to work with jupyter notebooks over the ssh connection. First, connect to the vmlab and configure a new conda environment as detailed below. Then clone the repo.

```bash
ssh $USER@vmlab.niu.edu
conda create -n columnar_env
conda activate columnar_env
conda install jupyterlab
pip install awkward uproot

git clone https://github.com/fstrug/C2P2sem2025-PythonExercises.git
```
Then we will start a jupyter lab session that we can connect to over some port. We will use port 8080, but any 8xxx port works.

```bash
jupyter lab --no-browser --port 8080
```

In a separate terminal, connect to the vmlab with the port used above for jupyter lab. Replace `$USER` with your username. 

```bash
ssh -L 8080:localhost:8080 $USER@vmlab.niu.edu
```

Copy and paste the URL from the first terminal window in a browser to 


Exercise results will be polled at [PollEv.com/frankstrug451](https://PollEv.com/frankstrug451).