# Not Valid for current implementation
# todo: rewrite

# treescore
Score a Christmas Tree based on uniformity of lights, shape of tree, and colors used.

Writeup with pretty pictures can be see at
http://christianreimer.github.io/treescore/

## Simple Example

```python
>>> from treescore import Treescorer
>>> fname = 'path/to/image/of/tree.png'
>>> treescorer = Treescorer(fname)
>>> treescorer.score()
>>> treescorer.scores
{'color': 72, 'light': 79, 'overall': 80.0, 'shape': 89}
>>> treescorer.imshow(treescorer.treedrawer.sketch())
>>>
```

This should display an image such as the following (depending on your tree of
course)
![original image](../readme/composite.png)


# Installation

OpenCV (http://opencv.org/) is used and you will need to install it. This will
probably be the biggest challenge you will encounter. You can follow the
instructions for python3 and OpenCV version 3 over at
http://www.pyimagesearch.com/opencv-tutorials-resources-guides

Once you have OpenCV and the python bindings installed, the rest should be as
easy as

```bash
$ mkvirtualenv treescore
$ git clone https://github.com/christianreimer/treescore.git
$ cd treescore
$ pip install requirements.txt
$ ./judge --help
$
```

