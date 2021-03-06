.. _plot_control_commands:

Plot Control Commands
=====================

These functions control the plotting characteristics of PyDV which affect all displayed curves.

.. note::
   **< >** = Required user input.

   **[ ]** = Optional user input.

   **[PyDV]:** = Python Data Visualizer command-line prompt.

annot
-----

Display text on the plot at point (x, y).

.. code::

   [PyDV]: annot <text> <x> <y>

**bkgcolor - 2.4**
------------------

Change the background color of the plot, window, or both

.. code::

   [PyDV]: bkgcolor <[plot | window] color-name | reset>

dashstyle
---------

Set the style of dash or dot dash lines. The python list is a list of integers, alternating how many pixels to turn on and off, for example:

    [2, 2] : Two pixels on, two off (will result in a dot pattern).

    [4, 2, 2, 2] : 4 on, 2 off, 2 on, 2 off (results in a dash-dot pattern).

    [4, 2, 2, 2, 4, 2] : Gives a dash-dot-dash pattern.

    [4, 2, 2, 2, 2, 2] : Gives a dash-dot-dot pattern.

    See matplotlib 'set_dashes' command for more information.

.. code::

    [PyDV]: dashstyle <curve-list> <[...]>

dataid
------

Show curve identifiers if True. **Alternative Form: data-id**

.. code::

   [PyDV]: dataid <on | off>

delannot
--------

Delete annotations from list.

.. code::

   [PyDV]: delannot <number-list-of-annotations>

domain
------

Set the domain for plotting. Using de (for default) will let the curves determine the domain.

.. code::

   [PyDV]: domain <low-lim> <high-lim>

                 OR

   [PyDV]: domain de

fontcolor
---------

Change the font color of given plot component.

.. code::

   [PyDV]: fontcolor [<component: xlabel | ylabel | title | xaxis | yaxis>] <color-name>

fontsize
--------

Change the font size of given component, or overall scaling factor.

.. code::

   [PyDV]: fontsize [<component: title | xlabel | ylabel | key | tick | curve | annotation>] <numerical-size | small | medium | large | default>

fontstyle
---------

Set the fontstyle family.

.. code::

   [PyDV]: fontstyle <serif | sans-serfif | monospace>

geometry
--------

Change the PyDV window size and location in pixels.

.. code::

   [PyDV]: geometry <xsize> <ysize> <xlocation> <ylocation>

grid
----

Set whether or not to draw grid lines on the graph. Default is off.

.. code::

   [PyDV]: grid <on | off>

guilims
-------

Set whether or not to use the GUI min/max values for the X and Y limits. Default is off.

.. code::

   [PyDV]: guilims <on | off>

handlelength
------------

Adjust the length of the line(s) in the legend.

.. code::

   [PyDV]: handlelength <length>

image
-----

Save the current figure to image file.

.. code::

   [PyDV]: image <file-name> <file-type: png | ps | pdf | svg>

label
-----

Change the key and list label for a curve.

.. code::

   [PyDV]: label <curve> <new-label>

labelFileNames
--------------

Change the key and list labels for all curves to append the filename.

.. code::

   [PyDV]: labelFileNames

latex
-----

Use LaTeX font rendering if True

.. code::

   [PyDV]: latex on | off

legend
------

Show/Hide the legend with on | off or set legend position with ur, ul, ll, lr, cl, cr, uc, lc. **Shortcuts: leg, key**

.. code::

   [PyDV]: legend <on | off> [position]

lnstyle
-------

Set the line style of the specified curves.

.. code::

   [PyDV]: lnstyle <curve-list> <style: solid | dash | dot | dotdash>

lnwidth
-------

Set the line widths of the specified curves. A line width of 0 will give the thinnest line which the host graphics system supports.

.. code::

   [PyDV]: lnwidth <curve-list> <width>

marker
------

Set the marker symbol and scale (optionally) for scatter plots. You can also use any of the matplotlib supported marker types as well. See the matplotlib documentation on markers for further information.

.. code::

   [PyDV]: marker <curve-list> <marker-style: + | . | circle | square | diamond> [marker-size]

movefront
---------

Move the given curves so they are plotted on top.

.. code::

   [PyDV]: movefront <curve-list>

range
------

Set the range for plotting. Using de (for default) will let the curves determine the range. **Shortcut: ran**

.. code::

   [PyDV]: range <low-lim> <high-lim> | de

style
-----

Use matplotlib style settings from a style specification. The style name of **default** (if
available) is reserved for reverting back to the default style settings.

.. code::

   [PyDV]: style <style-name>

ticks
-----

Set the maximum number of major ticks on the axes.

.. code::

   [PyDV]: ticks <quantity> | de

title
-----

Set a title for the plot

.. code::

   [PyDV]: title <title-name>

update
------

Update the plot after each command if True.

.. code::

   [PyDV]: update on | off

xlabel
------

Set a label for the x axis

.. code::

   [PyDV]: xlabel <label-name>

xlogscale
---------

Set log scale on or off for the x-axis. **Alternative Form: x-log-scale**, **Shortcut: xls**

.. code::

   [PyDV]: xlogscale <on | off>

xticks
------

Set the locations of major ticks on the x-axis

.. code::

   [PyDV]: xticks de | <number> | <list of locations> | <list of locations, list of labels>

xtickformat
-----------

Set the format of major ticks on the x axis. Default is plain.

.. code::

   [PyDV]: xtickformat <plain | sci | exp | 10**>

xticklength
-----------

Set the length (in points) of x ticks on the axis.

.. code::

   [PyDV]: xticklength <number>

xtickwidth
----------

Set the width (in points) of x ticks on the x axis.

.. code::

   [PyDV]: xtickwidth <number>

ylabel
------

Set a label for the y axis

.. code::

   [PyDV]: ylabel <label-name>

ylogscale
---------

Set log scale on or off for the y-axis. **Alternative Form: y-log-scale**, **Shortcut: yls**

.. code::

   [PyDV]: ylogscale <on | off>

ytickformat
-----------

Set the format of major ticks on the y axis. Default is plain.

.. code::

   [PyDV]: ytickformat <plain | sci | exp | 10**>

yticklength
-----------

Set the length (in points) of y ticks on the y axis.

.. code::

   [PyDV]: yticklength <number>

ytickwidth
----------

Set the width (in points) of y ticks on the y axis.

.. code::

   [PyDV]: ytickwidth <number>

yticks
------

Set the locations of major ticks on the y axis.

.. code::

   [PyDV]: yticks de | <number> | <list of locations> | <list of locations, list of labels>
