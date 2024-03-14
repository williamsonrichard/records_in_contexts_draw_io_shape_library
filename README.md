Records in Contexts shape library for draw.io
=============================================

Overview
--------

The file `records_in_contexts_shape_library.xml` defines a library of shapes for [draw.io](https://draw.io) for working graphically with [Records in Contexts](https://www.ica.org/resource/records-in-contexts-conceptual-model/). To be precise, the library provides a graphical semantics for [RiC-O](https://github.com/ICA-EGAD/RiC-O), the OWL ontology formally implementing Records in Contexts. It contains the following, in order:

* A single shape for literals
* A 'node' shape for each ontology class, split horizontally into two. The bottom half contains the ontology class name/id, whilst the top half is left blank: it is intended to be filled in by an individual name/id or IRI.
* An arrow for each object property.
* An arrow for each datatype property.

It is (hopefully!) complete, except that we for the moment have omitted 'relation classes' and object properties specifically pertaining to these; these classes and properties allow for a second (more verbose but also more flexible) pattern of use of RiC-O than the one the library so far covers, but the entirety of Records in Contexts is still to be found within the shape library for at least one pattern of use.

The object properties are sorted alphabetically, as are the datatype properties. The ontology classes are split into two: the 'entities' of Records of Contexts are presented first in the order they appear in the conceptual model, and then all other ontology classes are presented in alphabetical order.

Examples
--------

We include a few examples of graphs created using these shapes to illustrate the kinds of things possible. The symbol ⊂ means 'subproperty of' or 'subclass of'. Both screenshots and (in most cases) the underlying draw.io XML files, which can be imported into draw.io, are provided.



Feedback, bugs, suggestions
---------------------------

All very welcome! The 'Issues' tab in github can be used for bugs and suggestions. Otherwise I can be contacted at ricwil (at) arkivverket.no.


Typical uses
------------

A graphical semantics for an ontology is one that many find easier to understand and work with than a plain text representation. The shape library can be useful in any situation where one wishes to work with Records in Contexts without requiring knowledge of OWL: collaborative modelling or data addition, presentations, visualisation more generally, ... It is likely to be most appropriate for specific data: one record or record set and its properties, perhaps its relation to a few records or record sets, etc.

Draw.io is very flexible and powerful, and there are many ways to customise the graphs created using the shape library.



Planned directions
------------------

We intend to write something which can take a graph built using this shape library and generate a formalisation of it in OWL. In the other direction, one could define a graph template for certain kinds of data in draw.io, and programmatically populate the template from OWL data.


How to use
----------

[Import](https://www.drawio.com/blog/custom-libraries) the shape library into [draw.io](https://draw.io): go to File -> Open library from -> Device, and then, having downloaded `records_in_contexts_shape_library.xml` from this repository, select it. It may also work to use 'URL' and choose the link to the raw XML file in this repository.

Then simply drag and drop shapes from the library into the graph canvas and tweak and connect them as you wish. There are many shapes, but by hovering over it should be possible to quickly find what you are looking for; the labels (R001 for example) from the Records in Contexts conceptual model are provided to help with this, where a direct mapping exists.


License
-------

The shape library is made available without any restrictions at all, except that this unrestrictedness is not permitted to be invalidated/superseded/overridden in any way or to any degree.
