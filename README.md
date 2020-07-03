# Dark styles for Matplotlib

As a dark mode lover, I find the default Matplotlib dark plot unsatisfactory. So this is a collection of good dark themes for Matplotlib that I found on GitHub, along with installation instructions and usage snippets.

_Note:_ The line `%config InlineBackend.figure_format = 'retina'` is optional but it makes your plots high resolution in Jupyter notebooks.

## 1. Quantum Black

Source: https://github.com/quantumblacklabs/qbstyles

![qb-example](https://raw.githubusercontent.com/quantumblacklabs/qbstyles/master/examples/output_6_0.png)

### Installation

```
pip install qbstyles
```

### Usage

```
import matplotlib.pyplot as plt
import seaborn as sns
%config InlineBackend.figure_format = 'retina'
from qbstyles import mpl_style
mpl_style(dark=True)

#Plot here
```

You can change `dark=True` to `dark=False` for a good light theme, but why would you ever do that?

## 2. Pitaya Smoothie

Source: https://github.com/dhaitz/matplotlib-stylesheets

![pitaya-example](https://raw.githubusercontent.com/dhaitz/matplotlib-stylesheets/master/img/pitayasmoothie_dark.png)

### Usage

```
import matplotlib.pyplot as plt
import seaborn as sns
%config InlineBackend.figure_format = 'retina'
plt.style.use('https://github.com/dhaitz/matplotlib-stylesheets/raw/master/pitayasmoothie-dark.mplstyle')

##Plot here
```

## 3. Cyberpunk

Source: https://github.com/dhaitz/mplcyberpunk

![cyberpunk-example](https://raw.githubusercontent.com/dhaitz/mplcyberpunk/master/img/sin.png)

### Installation

```
pip install mplcyberpunk
```

### Usage

```
import matplotlib.pyplot as plt
import seaborn as sns
%config InlineBackend.figure_format = 'retina'
import mplcyberpunk
plt.style.use('cyberpunk')

#Plot here

mplcyberpunk.add_glow_effects()
```
## 4. Material Darker

Source: https://github.com/lewlin/material_darker_mpl

### Installation

1. Download `material_darker.mplstyle` from the linked repo into `~/.matplotlib/stylelib/` (create folder if necessary).
2. Make sure that `~/.matplotlib/stylelib/` is listed in the output of `sys.path` (callable from iPython).

### Usage

```
import matplotlib.pyplot as plt
import seaborn as sns
%config InlineBackend.figure_format = 'retina'
plt.style.use('material_darker')

#Plot here
```

## 5. Default dark background

![default-example](https://matplotlib.org/3.1.0/_images/sphx_glr_dark_background_001.png)
### Usage

```
import matplotlib.pyplot as plt
import seaborn as sns
%config InlineBackend.figure_format = 'retina'
plt.style.use('dark_background')

#Plot here
```
