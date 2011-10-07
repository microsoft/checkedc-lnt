.. _todo:

TODO
====

This is a TODO list of major and minor features for LNT.

Major Features
--------------

Too many to name!

Minor Features
--------------

Optimize test distribution format for common cases.

 1. We should left the test info higher in the format, so that it can easily be
 shared by a large number of samples.

 2. We should specify test samples in an array instead of objects, to avoid
 requiring repetitive 'Name' and 'Data' keys.

 3. We should support [test, sample] in addition to [test, [sample, ...]].

 4. If we changed the .success marker to be .failure, then having [test] be a
 shortcut for [test, 0] would be fairly nice, and in the visualization we would
 automatically get the right defaulting for absent tests.

These changes would significantly compact the archive format, which improves
performance across the board.