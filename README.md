### Dojo Bins were created to showcase unique methods of parametric modeling within Blender Geometry Nodes. The system takes simple data inputs like drawer size to output a unique layout of parametrically controlled bins that fill the space of the specified drawer.

#### "Red Bin" Version
Any bin scaled past size limit turns red indicating the bin is too large to be printed
![dojo-bins-scaling-gif](https://github.com/node-dojo/dojo-recursive-bins/assets/157924548/f287f265-a344-4d74-9c24-84e1e29d6697)

#### "2-step" Version
Any bin scaled past the size limit divides again. (still needs work)

![Screen Recording 2024-01-31 at 3 24 56 PM](https://github.com/node-dojo/dojo-recursive-bins/assets/157924548/b2241c28-45a2-4f5e-989a-210e691de739)

FEATURES:

- Parametric input parameters
- Live Print preview with "Layers"* and animated print previewing
- red bins = too big to print, blue bins = printable
- live dimensions on drawer and print preview


![print preview](https://github.com/node-dojo/dojo-recursive-bins/assets/157924548/771fb136-debb-4aa1-9b69-a0b4ac2e5f20)


MODIFIER PARAMETERS:
- Drawer Size
     x, y, z, dimensions
- Bin Gap Size
- Bin Wall Thiccness
- Bin Fillet
- divide x
- divide y
- Bin Select Preview
- Print Layer Preview
- Make Exportable.



WISHLIST/KNOWN ISSUES:
- layers in print preview are not accurate to real print layers. ideally they'd be parametrically calibrated and result reflected in the preview
- Wall thickness to be constrained to factors related to print nozzle size so that wall thiccness = number of passes per layer
- alternative methods of controlling oversized bins
     - automatically dividing bins that go over size
     - locking the scale of the bins to a maximum edge length of ~200mm (or whatever print bed build envelope is specified)
- allowing print bed size to be an input value
- allowing print nozzle to be an input value
- print output to pack as many possible bins onto print plate as possible (instead of the current 1 bin output method)
- freeze/save output of bin layouts
- add bin gap size as modifier parameter
- some values are arbitrary. tie them back to real world units when possible.
- make stackable!
- wall mountable?? you mad men. 
