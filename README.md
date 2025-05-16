# python-to-cpp
Python to C++ converter

This project was suggested for the "hack day" at [CW25](https://www.software.ac.uk/workshop/collaborations-workshop-2025-cw25). It was not selected as a project for the competition, but several people expressed an interest regardless.

[Original proposal](./docs/original.pdf)

## Aim
We want to be able to do this:
```
python converter.py -i file.py -o file.cpp --filetype script|lib
```
The generated C++ file would then need to be compiled before being run.

In theory, the ```converter.py``` tool could generate a C++ file which could do the same as itself, i.e.

```
python converter.py -i converter.py -o converter.cpp --filetype script
```
i.e. `converter.cpp` could be compiled into a `converter` executable which would do the same as `converter.py`. It will have to be seen whether this is possible or not.

## Previous and related work

[Pyxie compiler](https://sparkslabs.com/pyxie/) by Michael Sparks ([Previous iteration here](https://github.com/sparkslabs/microbit-prototype/tree/master/compiler))




