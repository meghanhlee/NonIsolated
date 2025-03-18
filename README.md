# NonIsolated

This is code associated to the preprint, [Isolated j-invariants arising from the modular curve X_0(n)](https://drive.google.com/file/d/1gGI4_JPJueaRvn_K2DodCv1Qt97zFdYs/view), by Meghan Lee.

The main function is 'NonIsolated', which given a non-CM, rational j-invariant, outputs a list <a_1, d_1>, ..., <a_n, d_n> of (level, degree) pairs which each correspond to a point of degree d_i on X_0(a_i) that is possibly isolated, and otherwise outputs an empty list if it determines that the j-invariant is not isolated. For some non-CM elliptic curve with the given j-invariant, we can compute a finite set of "primitive points" that is described in Section 5 in the paper, using the function 'PrimitiveDegreesOfPoints'. 

Installation instructions:
1. Install the latest version of Magma from [http://magma.maths.usyd.edu.au/magma/](http://magma.maths.usyd.edu.au/magma/).
2. Download David Roe's modified version of David Zywina's "OpenImage" repository from [https://github.com/roed314/OpenImage.git](https://github.com/roed314/OpenImage.git). Note that Magma version at least 2.27 is required to read the data files.
3. Download Jeremy Rouse, Andrew V. Sutherland, and David Zureick-Brown's "ell-adic-galois-images" from [https://github.com/AndrewVSutherland/ell-adic-galois-images](https://github.com/AndrewVSutherland/ell-adic-galois-images).
4. Attach the required files for the above repositories, by running
   ```
   AttachSpec("path/to/OpenImage/OpenImage.spec");
   Attach("path/to/ell-adic-galois-images/groups/gl2.m");
   ```
5. Download and run "NonIsolated.m" from https://github.com/meghanhlee/nonisolated.

Please contact us with any questions, comments, or suggestions.
