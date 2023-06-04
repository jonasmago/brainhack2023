---
jupytext:
  cell_metadata_filter: -all
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.10.3
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

(tipps)=
# Tipps and Tricks
**useful hacks, and notes for next iterations of this project**
- Plotting results
   - [plotly](https://plotly.com/)
   - histograms are powerful because they don't collapse either time or space 
   - raindrop plots are powerful as they show all individual points 
   - examples in the [python graph gallery](https://www.python-graph-gallery.com/)
- Python virtual environment
   - To make and actiavte a python virtual environment, use the following two lines:
      - `python3 -m venv venv`
      - `source venv/bin/activate`
   - To generate a `requirements.txt` file
      - Option 1: `pip freeze`.
      - Option 2: [Pipreqs](https://pypi.org/project/pipreqs/) automatically detects what libraries are actually used in a codebase. 
- Python local pip install 
   - make sure to have an __init__.py file in the src directory 
   - also make sure to have a setup.py file
   - Navigate to root directory and run: `pip install -e .`
- Python ipykernal allows to install kernals from python and conda environments 
   - `python -m ipykernel install --user --name=<my_env>`
- VIM: create and edit python files in the Terminal
   - `vim <file name>.py` 
   - `%s` search and replace
   - `i` insertion mode
   - doesn't leave a mess in the terminal after closing
   - alternative to `vim` is `nano`
- [Cookiecutter](https://www.cookiecutter.io/templates) as template for repos. 
   - [Teamplate for neuroimaging](https://github.com/patrickmineault/true-neutral-cookiecutter).
- Debugging scripst
   - `breakpoint()`can replace `import pdb; pdb.set_trace()``
   - `python -m pdb <script name>` runs a script with pdb. press `c` for continue when the script is loaded. This will allow you to be in the pdb when the code crashes. 
- [Neuro Maps](https://netneurolab.github.io/neuromaps/user_guide/nulls.html) allows to compare the pearsonr and p-value between two nifti files 
- The [Good Research Blog](https://goodresearch.dev/setup.html#install-a-project-package) shows how to do a local pip install (and much more)
- writing good code 
   - github copilot 
   - [sourcery](https://sourcery.ai/) automatically suggests improvements 
   - can I describe the function in **one** line

## About the Author
- `Name`: Jonas Mago
- `Contact`: jonas.h.mago@gmail.com
- `Affiliation`: McGill University
- `Background`: My background is in neuroimaging (EEG, fMRI), cognitive sciecnes, Active Inference, and Philosophy. After a BA in Liberal Arts and Sciences at the University College at Maastricht University and an MSc in Mind, Language, and Embodied Cognition at the University of Edinburgh, I am now pursuing my PhD at McGill University. 
- `General Interests`: I am using the Active Infernece framework to study the predictive and bayesian mechanics undrelying contemplative practices such as prayer, meditation, and psychedlics. Specifically, I work with (A) expert meditators from the Theravaden tradition that are able to enter absorption states called Jhana at will, (B) Charismatic Christian Prayer practitioners, and (C) experiences of entity encounters under the influnece of DMT. 

<div style="text-align: center;">
<a href="https://github.com/jonasmago">
   <img src="https://avatars.githubusercontent.com/u/57872952?s=400&u=6d910b22810b2a9d1f24be397cc71a279db91c87&v=4" width="150px;" alt=""/>
   <br /><sub><b>Jonas Mago</b></sub>
</a>
</div>