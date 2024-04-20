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

A graph created using the shape library can be parsed to formal OWL using a [command line tool](https://github.com/williamsonrichard/records_in_contexts_draw_io_parser) which we have written: see there for details.


Examples
--------

We include a few examples of graphs created using these shapes to illustrate the kinds of things possible. Two of the examples have been created directly using the shapes, whilst two have been created using the shapes but then elaborated manually upon. The symbol ⊂ means 'subproperty of' or 'subclass of'. Both screenshots and (in most cases) the underlying draw.io XML files, which can be imported into draw.io, are provided.


Coloured entities
-----------------

The file `records_in_contexts_shape_library--coloured_entities.xml` provides an alternative library in which the entities in RiC-O (with the prefix RiC-E in the conceptual model) are coloured according to the same scheme as that [chosen](https://groups.google.com/g/Records_in_Contexts_users/c/jvPTj01KmU0/m/oWs-ruaTGAAJ) by the developers of RiC-O. An entity which does not itself have a defined colour in this scheme has only its border coloured, in accordance with the entity which it is an immediate subclasses of.


Feedback, bugs, suggestions
---------------------------

All very welcome! The 'Issues' tab in github can be used for bugs and suggestions. Otherwise I can be contacted at ricwil (at) arkivverket.no.


Typical uses
------------

A graphical semantics for an ontology is one that many find easier to understand and work with than a plain text representation. The shape library can be useful in any situation where one wishes to work with Records in Contexts without requiring knowledge of OWL: collaborative modelling or data addition, presentations, visualisation more generally, ... It is likely to be most appropriate for specific data: one record or record set and its properties, perhaps its relation to a few records or record sets, etc.

Draw.io is very flexible and powerful, and there are many ways to customise the graphs created using the shape library.


How to use
----------

[Import](https://www.drawio.com/blog/custom-libraries) the shape library into [draw.io](https://draw.io): go to File -> Open library from -> Device, and then, having downloaded `records_in_contexts_shape_library.xml` or `records_in_contexts_shape_library--coloured_entities.xml` from this repository, select it. It may also work to use 'URL' and choose the link to the [raw XML file](https://raw.githubusercontent.com/williamsonrichard/records_in_contexts_draw_io_shape_library/main/records_in_contexts_shape_library.xml) of the shape library or its [coloured version](https://raw.githubusercontent.com/williamsonrichard/records_in_contexts_draw_io_shape_library/main/records_in_contexts_shape_library--coloured_entities.xml) in this repository.

Then simply drag and drop shapes from the library into the graph canvas and tweak and connect them as you wish. There are many shapes, but by hovering over it should be possible to quickly find what you are looking for; the labels (R001 for example) from the Records in Contexts conceptual model are provided to help with this, where a direct mapping exists.


Authors
-------

The original shape library is mainly due to myself, but evolved out of joint work with my colleague Trine Kruse. The version of the library with coloured entities is due to Trine, as is the coloured example. The other examples are due to the pair of us jointly.


License
-------

The shape library is made available without any restrictions at all, except that this unrestrictedness is not permitted to be invalidated/superseded/overridden in any way or to any degree.
