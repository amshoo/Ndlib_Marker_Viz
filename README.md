# Ndlib_Marker_Viz
Adding marker to Ndlib ComparisonViz and DiffusionViz to distinguish multiple lines and improve visual understanding.

NDlib is a Python software package that allows to describe, simulate, and study diffusion processes on complex networks. The package was design and documentation by GiulioRossetti you can find examples, tutorials and a complete reference here [ndlib](https://github.com/GiulioRossetti/ndlib).

Network Diffusion Library

## Adding a Marker To Ndlib Graph Viz

Matplotlib Marker: a basic matplotlib Marker plot, this shows a few optional features, like defining legend labels, legend size and maker size.
```python
Code to plot a simple demo with a “*” marker.
 
import matplotlib.pyplot as plt
x = [1,2,3,4,5]
fig, ax = plt.subplots()
ax.plot(x, '*' , markersize=12, label='(*)')
ax.axis('equal')
leg = ax.legend(fontsize=12);
```
Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.

## Usage

```python
import foobar

foobar.pluralize('word') # returns 'words'
foobar.pluralize('goose') # returns 'geese'
foobar.singularize('phenomena') # returns 'phenomenon'
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)