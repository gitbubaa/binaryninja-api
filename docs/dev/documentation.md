# Building Documentation

## CLA

To contribute to the Binary Ninja documentation, first sign the [contribution license agreement] and send it to [Vector 35].

## Prerequisites

- [sphinx]
- [breathe]
- [mkdocs]
- [doxygen]


## Building

### User/Help Documentation (Guides)

    git clone https://github.com/Vector35/binaryninja-api/
    cd binaryninja-api
    mkdocs build
The resulting documentation will be in `site/`

### Python API Documentation
    
    git clone https://github.com/Vector35/binaryninja-api/
    cd binaryninja-api
    cd api-docs
    make html
The resulting documentation will be in `api-docs/build/html`

### C++ API documentation
 
    git clone https://github.com/Vector35/binaryninja-api/
    cd binaryninja-api
Follow the `README.md` in `api-docs/cppdocs/`


## Changing
Changing documentation for the API itself is fairly straight forward. Use [doxygen style comment blocks](https://www.stack.nl/~dimitri/doxygen/manual/docblocks.html) in C++ and C, and [restructured text blocks](http://thomas-cokelaer.info/tutorials/sphinx/docstring_python.html) for python for the source. The user documentation is located in the `docs` folder and the API documentation is generated from the config in the `api-docs` folder.

!!! Tip "Tip"
    When updating the [User Documentation], the `mkdocs serve` will serve the webpages and watch for changes.

[contribution license agreement]: https://binary.ninja/cla.pdf
[Vector 35]: https://vector35.com/
[mkdocs]: http://www.mkdocs.org/
[breathe]: https://github.com/michaeljones/breathe
[sphinx]: http://www.sphinx-doc.org/en/stable/index.html
[doxygen]: https://www.doxygen.nl/index.html
[doxblocks]: doxygen
[User Documentation]: documentation.html#userhelp-documentation-guides