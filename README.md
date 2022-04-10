# adapted-prisms-periodicBCs

Here, sections of the code from PRISMS-Plasticity (https://github.com/prisms-center/plasticity) are adapted to allow for different numbers of mesh subdivisions in each direction when using periodic boundary conditions.

**What is PRISMS and where can the full code be found?**

PRISMS-Plasticity is a Finite Element Method (FEM) code developed based on the FEM librabry *deal ii*. PRISMS incorporates FEM models of crystal and continuum plasticity. The code can be found on the link
https://github.com/prisms-center/plasticity

**What is done in the adapted-prisms-periodicBCs?**

In the original PRISMS code for periodic boundary conditions, it is assumed that the mesh has the same number of elements in all directions (x, y and z). However, in some occasions it may be desired to vary the subdivions in each direction in a 3D simulation, such as to enforce a condition of plane strain loading while having fewer elements in the z-direction in order to save computational time. 
Here, in *adapted-prisms-periodicBCs*, you can find the files that are modified to allow such feature.

**Files modified from PRISMS:**
init.cc (src), periodicBCs.cc (src), ellipticBVP.h (include)
