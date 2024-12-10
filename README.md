# CUDA - Getting Started with PyTorch

## Introduction 
When machine learning with Python, you have multiple options for which library or framework to use. However, if you're moving toward deep learning, you should probably use either TensorFlow or PyTorch, the two most famous deep learning frameworks.

PyTorch is a powerful, yet easy-to-use deep learning library for Python, mainly used for applications such as computer vision and natural language processing.

While TensorFlow was developed by Google, PyTorch was developed by Facebook's AI Research Group, which has recently shifted management of the framework to the newly created PyTorch Foundation, which is under the supervision of the Linux Foundation.

The flexibility of PyTorch allows easy integration of new data types and algorithms, and the framework is also efficient and scalable, since it was designed to minimize the number of computations required and to be compatible with a variety of hardware architectures.


## Env Setup
Always start with a virtenv.
```shell
python -m venv venv
source venv/bin/activate
```
The rest operations are done in the virtual environment - `venv`.
## Install the python modules
Please install python modules: numpy, torch, and jupyter
```shell
pip install -r requirements.txt
```

## Verify the hardware
Just run:
```shell
python cua_verify.py
```

## CUDA Performance Test
Just run the code below, it may take a short while though.
```shell
python cuda_speedtest.py
```

## Notes
More details tests or practices? Please refer to the Jupyter Notebooks.
For sure, you have to run the Jupyter Notebook from here below
```shell
jupyter notebook
```
The system will ask for a token or password the first time you run the Jupyter Notebook. then you could copy the token part from the terminal windows since it will be something like:
> To access the server, open this file in a browser:
        file:///home/zenusr/.local/share/jupyter/runtime/jpserver-73812-open.html
    Or copy and paste one of these URLs:
        http://localhost:8888/tree?token=15d8832676224c0e0ebb1b9340abbe816ece71fbd4eaf288

Another way to disable the passpaswword and token is to run:
```shell
jupyter notebook --ip='*' --NotebookApp.token='' --NotebookApp.password=''
```

Here are the Notebooks for your reference:

- cuda_speedtest.ipynb
- PyTorch_Intro.ipynb

## License
MIT