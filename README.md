<h2>Second-Semester Synoptic Meteorology Labs</h2>
<h4><i>Release 1b, June 2023</i><br>Clark Evans and Michael Vossen</h4>

This repository contains a set of ten labs designed for a second-semester undergraduate course in synoptic meteorology, focusing on applying quasi-geostrophic theory, isentropic analysis principles, and isentropic potential vorticity concepts to better understand the lifecycle of midlatitude cyclones. Each lab is currently provided in Microsoft Word format, and each is supported by a Jupyter Notebook. 

The Jupyter Notebooks build on those from the <a href="https://github.com/evans36/SynopticMet1/"><b>first-semester synoptic meteorology course</b></a>, allowing students to grow in their ability to independently use Python tools to plot meteorological data. We highly recommend reviewing the first semester's labs and accompanying Jupyter Notebooks before beginning to dig into these labs.

If you are hosting a JupyterHub, or if your students have Jupyter Notebook installed locally (e.g., as part of an Anaconda Python distribution), then <a href="https://github.com/jupyterhub/nbgitpuller" target="_blank"><b>nbgitpuller</b></a> can be used to generate a link that downloads this repository into a working Notebook environment.

The Jupyter Notebooks cover the following topics:
<ul>
  <li><b>Lab 1</b>: Frontogenesis and Frontolysis</li>
  <li><b>Lab 2</b>: The Quasi-Geostrophic Vorticity Equation</li>
  <li><b>Lab 3</b>: The Quasi-Geostrophic Height-Tendency Equation</li>
  <li><b>Lab 4</b>: The Quasi-Geostrophic Omega Equation</li>
  <li><b>Lab 5</b>: Q Vectors</li>
  <li><b>Lab 6</b>: Cyclone Development in the Quasi-Geostrophic System via the Pettersen-Sutcliffe Development Equation</li>
  <li><b>Lab 7</b>: Isentropic Analysis</li>
  <li><b>Lab 8</b>: Isentropic Potential Vorticity Basics</li>
  <li><b>Lab 9</b>: Isentropic Potential Vorticity Anomaly Structures</li>
  <li><b>Lab 10</b>: Applications of Isentropic Potential Vorticity</li>
</ul>

Planned future additions/updates include:
<ul>
  <li>Adding the locally hosted datasets supporting each lab (excluding the ERA5 data that are provided with Lab 10). Alternatively, these data can be downloaded using the notebooks provided in the Scripts directory of the <a href="https://github.com/evans36/SynopticMet1/Scripts/"><b>first-semester synoptic meteorology repository</b></a>, or the notebooks may be rewritten to download the data straight from a cloud provider. We did not take this approach so as to avoid having ~10 local copies of the same (large) files.
  <li>Reworking each lab so that it is fully self-contained in Jupyter Notebooks. Some current lab elements, such as asking students to circle a feature or region on a map that is provided to them or that they create, are not well-suited to the current functionality of Jupyter Notebooks.</li>
  <li>Reworking labs which reference local data to reference cloud-based data. Since we use <a href="https://tljh.jupyter.org/en/latest/">The Littlest JupyterHub</a> for our local JupyterHub instance, we're currently stuck on Python 3.7. This has prevented us from updating the Notebooks to use the <a href="https://github.com/blaylockbk/Herbie">herbie</a> package's remote GRIB access and subsetting tools.</li>
</ul>

The primary packages used by these Jupyter Notebooks are cartopy, MetPy, siphon, and xarray. The JupyterHub on which these notebooks were first deployed runs Python 3.7.12, cartopy 0.20.0, MetPy 1.2.0, siphon 0.9, and xarray 0.20.2. It is likely that these notebooks will work with newer versions of each package with few, if any, changes.

Comments, questions, etc.: evans36-at-uwm-dot-edu.
