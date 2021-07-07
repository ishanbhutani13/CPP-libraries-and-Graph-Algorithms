# CPP-libraries- Segment Tree , Disjoint Union find
General purpose segment tree library and DSU.

include SegmentTree.h


to construct a segment tree you need to specify the following:

a. The datatype of array for which the tree is being constructed.

b. an array or vector for which the tree is to be constructed.

c. a value that can be used to fill the extra nodes of the tree.

d. a function combine that specifies how the result of left and right child of a node
should be used to generate the value of current node.

Example usage:

int small(int x,int y){return min(x,y);}
SegmentTree < int > rangeMinQueries(dataVector,INT_MAX,small);

int sum(int x,int y){return x+y;}
SegmentTree < int > rangeSumQueries(dataVector,0,sum);

long long product(long long x,long long y){return x*y;}
SegmentTree < long long > rangeProductQueries(dataVector,1,product);

union find data structure with union by rank and path compression heuristics To use the library:
include "DSU.h" in your source file.
following functionalities are provided:

a. construct DSU with n groups.

b. add new group to the DSU.

c. merge two existing groups.

d. find the root of the group to which an element belongs.

e. find number of elements in the group to which an element belongs.

Example usage : DSU myDSU(n);
