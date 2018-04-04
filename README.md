Thesis Plots
============

*Nice plot formatting for a scientific thesis* 

**Author:** John Garrett (https://github.com/garrettj403)

**Description:** This repo has two matplotlib style files that you can use to format plots for your thesis (or academic paper). The ``thesis`` style was optimized for singular plots (plots all on their own), while the ``subfigure`` style was optimized to fit two figures side-by-side (as a subfigure in LaTeX).

**Installation:** Put the ``*.mplstyle`` files in your Matplotlib style directory. If you're not sure where this is, in an interactive python console type:

```python
import matplotlib
matplotlib.get_configdir()
```

You should get back something like ``'/home/garrett/.matplotlib'``. You'd then put the ``*.mplstyle`` files in ``~/.matplotlib/stylelib/`` (you may need to create the ``stylelib`` directory). If your computer is like mine, you can use the Makefile contained within the repo to do this automatically.

**Use:** Whenever you want to use one of these styles, simply add the following to the top of your python script:

```python
import matplotlib.pyplot as plt 
plt.style.use('thesis')
# or
plt.style.use(['thesis','subfigure'])
```
Note that in the second case, the ``subfigure`` style will override some of the parameters from the ``thesis`` style.

Example
-------

![alt text](examples/figures/fig1.jpg)

**Note:** This looks a lot better as a PDF! See the ``examples/`` directory for more.
