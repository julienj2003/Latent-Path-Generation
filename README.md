# Latent-Path-Generation
### Master Thesis: Generative Models on Path Space - JOLY Julien, 2026.

---

## Abstract

Continuous-time generative models such as diffusion and flow matching have recently emerged as powerful tools for high-dimensional data generation. However, when applied to time series, these methods typically operate in discretized time space, ignoring the functional structure of trajectories.

In this work, we propose a spectral framework for generative modeling of time series based on a truncated Fourier representation. Rather than modeling paths pointwise, we learn diffusion and flow dynamics directly in coefficient space.

This representation yields a compact and orthogonal latent structure with an explicit decoding map, enabling stable training and efficient generation of long trajectories. Spectral truncation acts as an inductive bias, promoting smoothness while preserving the dominant dynamical modes of the data.

We evaluate the approach on synthetic oscillatory and dynamical systems, showing that both diffusion and flow matching models recover the statistical and structural properties of the underlying processes.

Our results demonstrate that embedding continuous-time generative models in structured functional bases provides a principled and scalable alternative to standard time-discretized formulations.

---

## Experiments

All experiments are ready to run and fully reproducible.

## How to Run

```bash
# Clone project
git clone https://github.com/julienj2003/Latent-Path-Generation.git
cd Latent-Path-Generation

# Install requirements
pip install -r requirements.txt
```


## Acknowledgements

The following GitHub repositories provided valuable and well-documented code bases:

https://github.com/Barb0ra/SigDiffusions

https://github.com/jsyoon0823/TimeGAN

https://github.com/atong01/conditional-flow-matching


## License

This project is licensed under the MIT License.

See the [LICENSE](LICENSE) file for details.

## Citation

If you use this work in your research, please cite:

```bibtex
@mastersthesis{yourlastname2026spectral,
  title     = {Generative Models on Path Space},
  author    = {Julien Joly},
  year      = {2026},
  school    = {ETH Zurich},
  type      = {Master's Thesis}
}
