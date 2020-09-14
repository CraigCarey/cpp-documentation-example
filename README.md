# cpp-documentation-example

https://github.com/TartanLlama/cpp-documentation-example

An example of setting up Sphinx for C++ and building with CMake and Read the Docs

See the documentation [here](https://cpp-documentation-example.readthedocs.io/en/latest/)

## Dependencies

- [CMake](https://cmake.org/download/)
- [Doxygen](http://www.doxygen.nl/download.html)
- [Sphinx](https://www.sphinx-doc.org/en/master/usage/installation.html)
- [Breathe](https://pypi.org/project/breathe/)
- [sphinx_rtd_theme](https://github.com/rtfd/sphinx_rtd_theme)

## Setup

Use python3 by default
```bash
sudo ln -sf /usr/bin/python3 /usr/bin/python
```

### Conda Setup
```bash
conda env create --file environment.yml
conda env create --file environment.yml --force  # if env already exists
conda activate docu-eval

conda deactivate
conda env remove -n docu-eval
```

## Installing Conda Packages
```bash
conda install -c conda-forge doxygen
```

## Building
```bash
mkdir build && cd build
cmake ../src
cmake --build .
```

## Building and Viewing Doxygen Generated Docs
```bash
cd docs/
doxygen
```
