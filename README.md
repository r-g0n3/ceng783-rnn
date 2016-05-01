# ceng783-rnn
CENG783 Term Project. Currently uses karpathy's char-rnn codes. These codes will be rewritten.

# Requirements
```
luarocks install torch
luarocks install nn
luarocks install optim
luarocks install nngraph
```
Optionally CUDA
```
luarocks install cutorch
luarocks install cunn
```
or OpenCL
```
luarocks install cltorch
luarocks install clnn
```

# Running
### Training 
Assumes data/some_folder/input.txt exists.
```
th train.lua -data_dir data/some_folder -rnn_size 512 -num_layers 2 -dropout 0.5 -gpuid -1
```

### Sampling
```
th sample.lua cv/some_checkpoint.t7 -gpuid -1
```
