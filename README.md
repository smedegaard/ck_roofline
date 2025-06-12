# How to Use

install [`uv`](https://docs.astral.sh/uv/) 

run `uv venv` inside the project folder

activate the virtural environment with `source .venv/bin/activate`. If you use another shell than bash add `[.bat/.csh/.fish/.nu/.ps1]`. example: `source .venv/bin/activate.fish` for Fish Shell.

Register your virtual environment as a Jupyter Kernel by running the following from within the activated virtual environment:

`python -m ipykernel install --user --name ck-roofline --display-name "Python (CK Roofline)"
`

start jupyter lab with `uv run --with jupyter jupyter lab`

Now you should be able to choose the python kernel in the to pright corner of the Jupyter interface on the nootbook roofline.ipynb. All dependencies defined in `pyproject.toml` should be installed when running `uv venv`.