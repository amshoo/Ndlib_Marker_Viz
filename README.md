# Ndlib_Marker_Viz
Adding marker to Ndlib ComparisonViz and DiffusionViz to distinguish multiple lines and improve visual understanding.

NDlib is a Python software package that allows to describe, simulate, and study diffusion processes on complex networks. The package was design and documentation by GiulioRossetti you can find examples, tutorials and a complete reference here [ndlib](https://github.com/GiulioRossetti/ndlib).

Network Diffusion Library

## Adding a Marker To Ndlib Graph Viz

Matplotlib Marker: a basic matplotlib Marker plot, this shows a few optional features, like defining legend labels, legend size and maker size.
```python
#Code to plot a simple demo with a “*” marker.
 
import matplotlib.pyplot as plt
x = [1,2,3,4,5]
fig, ax = plt.subplots()
ax.plot(x, '*' , markersize=12, label='(*)')
ax.axis('equal')
leg = ax.legend(fontsize=12);
```
Below are some basic example plots for markers.

## Assign a unique markers for each plot

Form [Solution 4](hhttps://stackoverflow.com/questions/13091649/unique-plot-marker-for-each-plot-in-matplotlib)in stackoverflow, which answer the quatio of how to us unique markers for each plot in matplotlib. the solution uses ‘itertools.cycle’ to iterate over a list or tuple indefinitely which picks markers randomly for you. The answer shown blow. 

Python 2.x

```python
import itertools
marker = itertools.cycle((',', '+', '.', 'o', '*')) for n in y:
    plt.plot(x,n, marker = marker.next(), linestyle='')
```
Python 3.x

```python
import itertools
marker = itertools.cycle((',', '+', '.', 'o', '*')) for n in y:
plt.plot(x,n, marker = next(marker), linestyle='')
```

To find the set of All possible markers you can visit matplotlib.markers[2] in matplotlib website (https://matplotlib.org/3.1.0/api/markers_api.html).

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
