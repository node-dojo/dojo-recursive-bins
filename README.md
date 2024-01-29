
![dojo-bins-scaling-gif](https://github.com/node-dojo/dojo-recursive-bins/assets/157924548/eb0de725-b7d9-4530-8200-9e71da6555b7)

Dojo Bins were created to showcase unique methods of parametric modeling within Blender Geometry Nodes. The system takes simple data inputs like drawer size to output a unique layout of parametrically controlled bins that fill the space of the specified drawer.


![print-preivew-grow](https://github.com/node-dojo/dojo-recursive-bins/assets/157924548/4c7997f9-5239-4caf-a2ac-6e93274c75b2)

FEATURES:

Parametric input parameters listed below
Live Print preview with "Layers"* and animated print previewing
red bins = too big to print, blue bins = printable

MODIFIER PARAMETERS:
- Drawer Size
     x, y, z, dimensions
- Bin Wall Thiccness
- Bin Fillet
- divide x
- divide y
- Bin Select Preview
- Print Layer Preview
- Make Exportable.

![Screenshot 2024-01-29 at 11 52 24 AM](https://github.com/node-dojo/dojo-recursive-bins/assets/157924548/e07e3452-526b-471a-aeae-423f5406533b)

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
