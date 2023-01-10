# tensorflow-digits

Classic Tensorflow project - handwritten digit recognition 

Using mnist dataset

Developed on Python 3.9 in Ubuntu using WSL2

To enable GPU processing, follow: https://www.tensorflow.org/install/pip#windows-wsl2_1

## Running with conda

Recommended to use conda for tensorflow-gpu
`conda env create -f environment.yaml`
`conda activate tf`
`python3.9 main.py`

To export use:
`conda env export > environment.yaml`

## Test tensorflow cpu
`python3.9 -c "import tensorflow as tf; print(tf.reduce_sum(tf.random.normal([1000, 1000])))"`

## Test tensorflow gpu
`python3.9 -c "import tensorflow as tf; print(tf.config.list_physical_devices('GPU'))"`

## Running tensorboard
`tensorboard --logdir logs/fit`
