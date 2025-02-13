# Photo-morphism-tool
A photo morphism tool for morphing 3 images instead of 2

So many of us have used photo morphism for several purposes right? Well, I always wanted to morph more than 2 images at a time, so I changed the formula of morphing 2 images a little bit, so that we can now morph 3 images together :)

The formula is given below:

For three images A, B, and C, the generalized morphing formula would be:

M(x,y) = (1−t1−t2) ⋅ A(x,y) + t1 ⋅ B(x,y) + t2 ⋅ C(x,y) 

Where:
M(x,y): The resulting pixel value at position (x,y) in the morphed image.
A(x,y), B(x,y),C(x,y): Pixel values at position (x,y) in images A, B, and C, respectively.
t1​ and t2: Blending parameters for images B and C, respectively.
(1−t1−t2): Weight for image A, ensuring the total weight is 1 (to preserve brightness levels).

Constraints:
To maintain a valid blend, the parameters should satisfy:
t1 ≥ 0,  t2 ≥ 0,  t1 + t2 ≤ 1

How It Works:
If t1 = t2 = 0: The result is entirely A(x,y).
If t1 = 1 and t2 = 0: The result is entirely B(x,y).
If t1 = 0 and t2 = 1: The result is entirely C(x,y).
If 0 < t1, t2 < 1: The result is a smooth blend of A, B, and C.



How to run the Code:

Well, the code is pretty simple and easy to run, make sure you have OpenCV and numpy, along with software like R studio or something similar to adjust the trackbars in the images. Simply copy-paste the code on your PC and run in any python environment. Enjoy :)
