CntInDegNodes
'''''''''''''''''''

.. function:: CntInDegNodes(Graph, NodeInDeg)

Returns the number of nodes with in-degree NodeInDeg.

Parameters:

- *Graph*: graph (input)
    A Snap.py graph or a network

- *NodeInDeg*: int (input)
    The value of in-degree to be found in *Graph*

Return value:

- TInt (output)
	Integer with the number of nodes with in-degree equals to *NodeInDeg*


The following example shows how to use CntInDegNodes for Graphs in
:class:`TNGraph`, :class:`TUNGraph`, and :class:`TNEANet`::
    
	import snap

    Graph = snap.GenRndGnm(snap.PNGraph, 100, 1000)
    nodeCount = snap.CntInDegNodes(Graph, 10)
    print nodeCount

    Graph = snap.GenRndGnm(snap.PUNGraph, 100, 1000)
    nodeCount = snap.CntInDegNodes(Graph, 20)
    print nodeCount

    Graph = snap.GenRndGnm(snap.PNEANet, 100, 1000)
    nodeCount = snap.CntInDegNodes(Graph, 5)
    print nodeCount