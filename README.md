# porousCFoam
This is a code for porous media dissolution using a Darcy-Brinkman flow solver. 

It is designed to have user programmable constitutive models, examples of which are in the Models subdirectory. 

Now supports multiple mineral and concentration fields; the algorithm is explained in rates.pdf.

The external pressure gradient should always be in the x direction. There are some sample cases in porousCases_v3, which has its own README. The sole input fields are the mineral fractions F0, F1, etc. although other fields (p, U, Cx) need to be initialized and their boundary conditions defined; this is taken care of automatically once the number of each species is specified (system/porousFoamDict)
