# Conda
* ERROR  
PackagesNotFoundError: The following packages are not available from current channels:
```
ResolvePackageNotFound:
  - cudatoolkit=11.3
```
* Solution
```
conda install cudatoolkit=11.3 -c pytorch -c conda-forge
```
