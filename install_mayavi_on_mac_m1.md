# Install mayavi on MacBook Pro M1

by: https://github.com/walkoncross (zhaoyafei0210@gmail.com)

## Install vtk
```
pip3 install vtk==9.0.2
```

## Install PyQt5

```
pip install PyQt5
```
If pip install failed (which did on my Mac), install from Homebrew:

```
brew install PyQt5
```
and make symbol link:
```
ln -s /opt/homebrew/Cellar/pyqt@5/5.15.4_2/lib/python3.9/site-packages/PyQt /Users/zhaoyafei/miniforge3/lib/python3.9/site-packages
```
Replace "/Users/zhaoyafei/miniforge3/lib/python3.9/site-packages" with your python lib path.

## Install mayavi from source
```
git clone https://github.com/enthought/mayavi.git
cd mayavi
python setup.py install
```