The quest for measuring myelin with MRI - An interactive meta-analysis
======================================================================

_Matteo Mancini, Agah Karakuzu, Thomas Nichols, Julien Cohen-Adad, Mara Cercignani, Nikola Stikov_

<br>

This repository generates the interactive figures and the meta-analysis results for our study "The quest for measuring myelin with MRI – An interactive meta-analysis of quantitative comparisons with histology".

###  📎[The full preprint is available on bioRxiv.](https://www.biorxiv.org/content/10.1101/2020.07.13.200972v2)


## 🖥 Usage instructions 

This Jupyter Book is published by NeuroLibre at <a href="https://neurolibre.github.io/myelin-meta-analysis">https://neurolibre.github.io/myelin-meta-analysis</a>, where all the interactive content is made readily available!

However, several options are available if you would like to reproduce the outputs
by re-executing the code. 

<details><summary> <b>💻 Execute locally</b> </font> </summary><br>

The required packages can be installed using pip:

```
pip install -r requirements.txt
```
---
**Note:**

R and the metafor package are both needed to fit the mixed-effect model in `meta-analysis.ipynb` through the package rpy2.

---
</details>

<details><summary> <b>🐳 Use with Docker</b> </font> </summary><br>

If you have Docker installed on your computer and running, you can run the code 
in the same environment described in this repository using `repo2docker`. 

1. Simply install `repo2docker` from pyPI: 
```
pip install jupyter-repo2docker
```
2. Run the following command in your terminal:
```
jupyter-repo2docker https://github.com/neurolibre/myelin-meta-analysis
```

After building (it might take a while!), it should output in your terminal 
something like:

```
Copy/paste this URL into your browser when you connect for the first time,
    to login with a token:
        http://0.0.0.0:36511/?token=f94f8fabb92e22f5bfab116c382b4707fc2cade56ad1ace0
```

This should start a Jupyter session on your browser and make all the resources 
you see when you [launch a Binder](https://mybinder.org/v2/gh/neurolibre/myelin-meta-analysis/master) for this repository. 

To re-use your container built by repo2docker, do the following: 

1. Run `docker images` command and copy the `IMAGE ID` to your clipboard 
2. Run the following command to start the container:
```
docker run -it --rm -p 8888:8888 `PASTE IMAGE ID HERE` jupyter notebook --ip 0.0.0.0
```

If `jupyter-repo2docker` does not work, you can download the Docker Image .zip file found [here](https://zenodo.org/record/6463437#.Y18pbC8r1pR) and follow the instructions. 

You can even use a volume in order to open a local (and therefore, mutable) directory in the container of interest by adding the `-v ` flag to your `docker run` command:

`docker run -v PATH_TO_LOCAL_DIR:PATH_TO_LOCAL_DIR_IN_CONTAINER -it --rm -p 8888:8888 `PASTE IMAGE ID HERE` jupyter lab --ip 0.0.0.0`

</details>

<details><summary> <b>☁️ Zero installation</b> </font> </summary><br>

You can use <code> Interact Inline </code> or <code>Launch in Binder</code> buttons 
at the top of each page of the <a href="https://neurolibre.github.io/myelin-meta-analysis">Jupyter Book</a>.

Alternatively, you can start a Binder session by clicking the badge below: 

[![Binder](https://github.com/zelenkastiot/binder_badges/blob/master/badges/myelin--meta--analysis-binder.svg)](https://mybinder.org/v2/gh/neurolibre/myelin-meta-analysis/master)

</details>

## 🧬 Contribute to Living Meta-Analysis
First, make sure that your meta-analysis passes all of the exclusion criteria listed below.
<details><summary> <b>Level 1 Exclusion Criteria</b> </font> </summary><br>
- work relying only on MRI;
- work relying only on histology or equivalent approach;
- work does not compare MRI data to histology data or reports only qualitative comparisons.
</details>
<details><summary> <b>Level 2 Exclusion Criteria</b> </font> </summary><br>
- studies using MRI-based measures in arbitrary units;
- studies using measures of variation in myelin content;
- studies using arbitrary assessment scales;
- studies comparing absolute measures of myelin with relative measures;
- studies reporting other quantitative measures than correlation or R^2 values;
- studies comparing histology from one dataset and MRI from a different one.
</details>
<details><summary> <b>Level 3 Exclusion Criteria</b> </font> </summary><br>
- not providing an indication of both number of subjects and number of ROIs;
- not brain;
- ROIs as distinct samples;
- ROIs of only 1 voxel.
</details>
<details><summary> <b>Next, provide us with the following information:</b> </font> </summary><br>
- DOI
- First author
- Year
- Approach	
- Magnetic field
- MRI measure(s)
- Histology/microscopy measure
- Tissue condition
- Human/animal
- Condition
- Focus	
- Specific structure(s)
- Comparison
- Subjects
- M/F
- ROI per subject
- Co-registration
- Control group	
- Notes							
<br>

<hr>
<p align="center">
<img src="https://avatars3.githubusercontent.com/u/63861117?s=200&v=4" style="width:40px;"></img> <br>
This repository is created by <a href="https://github.com/Notebook-Factory">Notebok-Factory</a>. 
</p>
