# General Relativity

Python notebooks to compute items of interest in General Relativity, such as Christoffel symbols, Reimann and Ricci tensors, and the Ricci scalar.

There is currently one Python notebook in this repository, named `Tensor Calculator - General Relativity.ipynb`, with more to potentially be added in the future.

Current dependencies required:
* [SymPy](https://docs.sympy.org/latest/install.html)


## Tensor Calculator Notebook

A simple easy-to-use Jupyter Notebook to help compute Christoffel symbols, the Reimann and Ricci tensors, and the Ricci scalar using SymPy with a given spacetime metric in 3 + 1 dimensions.

This Python notebook allows you input your metric, the symbols (variables) that your metric depends on (in order), and the initial orientation of your metric (whether you have g<sub>μν</sub> or g<sup>μν</sup>).

To view your metric in a matrix form, use `gtensor`.

To view all possible Christoffel symbols in a 4x4x4 matrix, use `ChristoffelSymbols(metric)`.

To view a specific Christoffel symbol, i.e. Γ<sup>3</sup><sub>23</sub>, use `GiveChristoffel(3,2,3,metric)`, where the first number, 3, is the upper index and 2 and 3 are the two lower indices in order.

To view the Reimann tensor in a 4x4x4x4 matrix, use `ReimannTensor(metric)`.

To view a specific component of the Reimann tensor, i.e. R<sup>1</sup><sub>313</sub>, use `GiveReimann(1,3,1,3,metric)`, where the first number, 1, is the upper index and 3, 1, and 3 are the three lower indices in order.

To view the Ricci tensor in a 4x4 matrix, use `RicciTensor(metric)`.

To view a specific component of the Ricci tensor, i.e. R<sub>33</sub>, use `GiveRicci(3,3,metric)`, where the numbers correspond to the two lower indices in order.

Lastly, to compute the Ricci scalar for the metric, simply use `RicciScalar(metric)` to get the Ricci scalar.

More information, instructions, and examples are in the notebook. 
