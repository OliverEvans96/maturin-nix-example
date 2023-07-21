# maturin-nix-example

This is an example of building a rust package with python bindings using maturin/pyo3 via the nix package manager (with crane).

## Usage

You should be able to build and test the package without even cloning the repo, using:
```
$ nix run github:oliverevans96/maturin-nix-example
```

which will put you in an IPython shell, where the package can be imported and used:
```python
Python 3.10.12 (main, Jun  6 2023, 22:43:10) [GCC 12.2.0]
Type 'copyright', 'credits' or 'license' for more information
IPython 8.11.0 -- An enhanced Interactive Python. Type '?' for help.

In [1]: import testpkg

In [2]: testpkg.sum_as_string(3, 5)
Out[2]: '8'
```
