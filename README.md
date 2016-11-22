# trisdesclous : spike sorting with [french touch](https://fr.wikipedia.org/wiki/French_touch_(informatique)).

**tris des clous** is a very dishonest translation of **spike sorting** to french.

Pronouce it [tree day clue] for english speaker.

Documentation is here: http://tridesclous.readthedocs.io/

This module provide some functions and examples of spike sorting.
It is our material to teach good practices in spike sorting technics.

You can also use it for real data of course. Be courious and try it.
The forest of spike sorting tools is dense and *tridesclous* is a new tree.

*tridesclous* is a complete rewrite of our old (and unsuccessful) tools (SpikeOmatic, OpenElectrophy, ...)
with up-to-date (in 2015) python modules to simplify our codes.

tridesclous:
  * should make easy to leave a mark of your spike sorting process in
    a jupyter notebook.
  * offer a simple UI written in Qt for interactive exploration.
  * could be usefull for online spikesorting in a near futur with pyacq.

In short, *tridesclous* force you to write a script for spike sorting but 
you also benefit of a simple UI for offline spike sorting (and online soon).

Bonus:
  * Some pieces of algorithm of written both in pure python (numpy/scipy/...) and OpenCL (filter, peak detetion, ...). So *tridesclous* should be efficient for large array (>=64 channel) soon.
  * Each piece of the algorithm is written with chunk by chunk in mind. So the offline *tridesclous* is not agressive for memory.
  
  
  

Dependencies:
  * numpy
  * pandas
  * sklearn
  * scipy
  * matplotlib
  * seaborn
  * PyQt4 (for UI only)
  * pyqtgraph (for UI only)
  * jupyter (for UI only)
  * pyacq (for online)

For test:
  * pytest

This is in construction so for easy install/update do:
```
git clone https://github.com/tridesclous/tridesclous.git
cd tridesclous
python setup.py develop
```

while tridesclous is not installed but linked, for having new version just do:
```
git pull
```



Authors: Christophe Pouzat and Samuel Garcia


![snapshot](doc/img/snapshot_cataloguewindow.png)
![snapshot](doc/img/snapshot_peelerwindow.png)
