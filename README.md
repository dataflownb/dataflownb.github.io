Dataflow notebooks are Jupyter notebooks written in Python that use a modified kernel (dfkernel) to enable new features. Specifically,

* Cells have persistent identifiers, allowing any output to be robustly referenced (e.g. `Out[a32b3f]`)
* By leveraging the cell identifiers, any cell execution will recursively update any referenced cells that have changed just like dataflows which update upstream modules as needed
* There is no need to order cells so that dependent cells are before the cell that uses them
* Navigation is enhanced by links to referenced cells and directed graph visualizations of the induced dataflow
* Intermediate outputs are both viewable via the rich Jupyter output formats and usable in later cells
* Dataflow notebooks can be converted to standard python notebooks 

Projects:

* [dfkernel](github.com/dataflownb/dfkernel): a Jupyter kernel that provides dataflow features
* [dfconvert](github.com/dataflownb/dfconvert): a script to transform ipynb files created using the dataflow kernel to a standard python notebook
