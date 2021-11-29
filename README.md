pyside2uic
=========

Provides PySide2 dynamic .ui file loading similar to the PyQt5 uic functionality.


Installation
------------

```sh
python3 -m pip install git+https://github.com/turboss/pyside2uic.git
```

Usage
-----

The `loadUi()` function takes a path to .ui file and an object to load it onto.

```python
from PySide import QtGui
from pyside2uic import loadUi

class MyWidget(QtGui.QWidget):

    def __init__(self, *args, **kwargs):
        super(MyWidget, self).__init__(*args, **kwargs)
        loadUi('mywidget.ui', self)

```
