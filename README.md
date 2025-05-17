# python-to-cpp
Python to C++ converter

This project was suggested for the "hack day" at [CW25](https://www.software.ac.uk/workshop/collaborations-workshop-2025-cw25). It was not selected as a project for the competition, but several people expressed an interest regardless.

[Original proposal](./docs/original.pdf)

## Motivation 
C++ programs run faster than Python, so are likely to use less energy, e.g., on an HPC system. There is also some evidence that C++ programs use less power (see original proposal). So, it is desirable to use C++.

But much existing code is written in Python. And, many programmers don't know C++.

The idea of this project is to develop a tool which can convert Python source code to C++ source code, which can then be compiled and run. In theory, this would allow programmers to run C++ code even if they don't know C++. And programmers, whether they know C++ or not, could "convert" an existing Python code base into C++.

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

* [Pyxie compiler](https://sparkslabs.com/pyxie/) by Michael Sparks ([Previous iteration here](https://github.com/sparkslabs/microbit-prototype/tree/master/compiler))
* [SWIG](https://www.swig.org/)
* [Python `ast` module](https://docs.python.org/3/library/ast.html)
* [FLAME GPU 2](https://github.com/FLAMEGPU/FLAMEGPU2)




