MeshResampling
==============

**Description**

Reducing number of faces while trying to keep overall shape, volume and
boundaries You can specify a fixed, min, max Vertices number.

This is different from MeshDecimate!

Resampling
``https://users.cg.tuwien.ac.at/stef/seminar/MeshResamplingMerge1901.pdf``

settings

================================= ======================================================================================================================================================================
Name                              Description
================================= ======================================================================================================================================================================
Input                             Input Mesh (OBJ file format)
Simplification factor             Simplification factor 0.5 ``(0 - 1)``
Fixed Number of Vertice           Fixed number of output vertices 0 ``(0 - 1 000 000)``
Min Vertices                      Min number of output vertices 0 ``(0 - 1 000 000)``
Max Vertices                      Max number of output vertices 0 (0 - 1 000 000)
Number of Pre-Smoothing Iteration Number of iterations for Lloyd pre-smoothing 40 (0 - 100)
Flip Normals                      Option to flip face normals. It can be needed as it depends on the vertices order in triangles and the convention change from one software to another. (True/False)`\`
Verbose Level                     ['fatal', 'error', 'warning', 'info', 'debug', 'trace']
Output mesh                       Output mesh (OBJ file format) ``internalFolder + mesh.obj``
================================= ======================================================================================================================================================================

|image0|

**Comparison MeshDecimate and MeshResampling**

|image1|

**Flip Normals**

|image2|

.. |image0| image:: mesh-resampling.jpg
   :target: mesh-resampling.jpg
.. |image1| image:: compare-resampling-decimate.jpg
   :target: compare-resampling-decimate.jpg
.. |image2| image:: flip-normals.jpg
   :target: flip-normals.jpg
