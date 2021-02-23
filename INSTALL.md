- Download and install CUDA 11
- `export PATH="/usr/local/cuda/bin:$PATH"`
- `export LD_LIBRARY_PATH="/usr/local/cuda/lib64:$LD_LIBRARY_PATH"`
- Create new conda environment with `python=3.7`
- Install PyTorch, because of [this bug](https://github.com/pytorch/pytorch/issues/51080) either with
`conda install pytorch torchvision cudatoolkit==11.0.3 -c pytorch -c conda-forge` or `pip install --pre torch torchvision -f https://download.pytorch.org/whl/nightly/cu110/torch_nightly.html`
- Install remaining dependencies: `pip install click requests tqdm psutil scipy pyspng ninja imageio-ffmpeg==0.4.3`
