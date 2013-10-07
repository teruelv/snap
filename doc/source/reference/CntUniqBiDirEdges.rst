CntUniqBiDirEdges
'''''''''''''''''

.. function:: CntUniqBiDirEdges(Graph)

Counts unique bidirectional edges in the graph Graph. Edge is bidirectional if there exists directed edges in both directions: (u,v) and (v,u).

Parameters:

- *Graph*: graph (input)
    A Snap.py graph or a network

Return value:

- Integer value

For more info see: http://snap.stanford.edu/snap/doc/snapdev-ref/index.html

The following example shows how to calculate CntUniqBiDirEdges for edges in
:class:`TNGraph`, :class:`TUNGraph`, and :class:`TNEANet`::

    import snap

    Graph = snap.GenRndGnm(snap.PNGraph, 100, 1000)
    print "Directed Graph: Count of Unique Bidirectional Edges is %d" % (snap.CntUniqBiDirEdges(Graph))

    Graph = snap.GenRndGnm(snap.PUNGraph, 100, 1000)
    print "Undirected Graph: Count of Unique Bidirectional Edges is %d" % (snap.CntUniqBiDirEdges(Graph))

    Graph = snap.GenRndGnm(snap.PNEANet, 100, 1000)
    print "Network Graph: Count of Unique Bidirectional Edges is %d" % (snap.CntUniqBiDirEdges(Graph))