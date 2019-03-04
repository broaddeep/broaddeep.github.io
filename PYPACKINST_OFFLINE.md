# Question: how to install the python package in the offline mode?

- download pack and all the dependencies by

```
pip download package-you-want-to-install
```

- assuming you are in the directory 
- filled with all the dependencies of the package you want to install.
- --no-index : ignores package index (only looking at --find-links URL instead) 
- --find-links : if a local path or file:// url, then look for achives in the directory listing

```
pip install --no-index --find-links="." package-you-want-to-install.tar.gz
```

```python
print("enjoy")
```
