# jupyter-park

## Setup env
```bash
python3 -m venv env
```

## Start env
```bash
source env/bin/activate
```

## Start jupyter
```bash
jupyter lab
```

## Close env
```bash
deactivate
```

## Install Rust kernel from source
```bash
git clone git@github.com:evcxr/evcxr.git
cd evcxr
cargo install --locked evcxr_jupyter
evcxr_jupyter --install
```

> ⚠️ **_WARNING:_** Run jupyter lab at least once before installing the Rust kernel. The last command depends on there already being the folder  `~/.local/share/jupyter`.  

## Install Rust source code
```bash
rustup component add rust-src
``` 

