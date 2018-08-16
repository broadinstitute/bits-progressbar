# bits-progressbar

BITS Progressbar Package

## Install

`pip install bits-progressbar`

## Use

### Progress bar for a list of items
```
from bits.progressbar import Progress

my_list = ['list', 'of', 'items', 'to', 'process']

progress = Progress().start(my_list, verbose=True)
for item in mylist:
    progress.update()
    # do some stuff
progress.finish()
```
from bits.progressbar import Progress


# Progress timer for an unknown list of items
```
from bits.progressbar import Progress

mylist = []

progress = Progress().start(verbose=self.verbose)
while True:
    progress.update(mylist)
    # do some stuff to add items to mylist
progress.finish(mylist)
```
