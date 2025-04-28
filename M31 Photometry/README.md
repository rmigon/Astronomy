# Rafael Vieira Migon

## Photometry of a Spiral Galaxy

2024.2 Semester

### Study Object

In this module, I explored image analysis using packages like NumPy, SciPy, and Astropy. For this project, I chose to work with a well-known elliptical galaxy to practice photometric analysis of a non-circular object. Using SAOImage DS9 software, I obtained a 10-arcminute cutout around the Andromeda Galaxy (Messier 51, RA 00:42:44.3 — Dec +41° 16' 9") in FITS format to load into a Jupyter Notebook.

### Objective

Analyse the total flux from the Andromeda Galaxy in the image, taking into account potential background noise.

### Analysis Plan

Analysing a circular object can be straightforward since the shape is well-defined and easy to deduce. An elliptical object introduces additional parameters that need to be analysed to achieve satisfactory results. 

Using SciPy, NumPy, and Astropy packages, the galaxy image will be loaded into a Jupyter Notebook. The pixels provide information about the flux in the study region. For the ellipse, I will use the form:

(x - x₀)²/a² + (y - y₀)²/b² = 1

Where:
- `x₀` and `y₀` are coordinates for the ellipse center
- `a` and `b` are the semi-major and semi-minor axes

For the photometric analysis, I will use concepts like:
- Moment of inertia
- Signal-to-Noise Ratio (SNR), defined as:

S/N = Nₑ/√[Nₑ + n_pix × (Nₛ + N_D + N_R)]

Where:
- `Nₑ`: Counts due to the light source
- `Nₛ`: Counts due to sky background brightness
- `N_D`: Counts due to dark current ≈ 0 (corrected with Dark Frames)
- `N_R`: Counts due to read noise ≈ 0 (corrected with Bias Frames)
- `n_pix`: Number of pixels being counted

### References

1. Andromeda Galaxy (Wikipedia)
2. Semi-major and Semi-minor Axes (Wikipedia)
