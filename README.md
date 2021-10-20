## graphDB
Similer to tables in Relational datbases we have vertices and edges in the graph database.
Vertex - Analoges to a table.So each vertex contains a particular sub set of information.
Attributes- In a vertex we have are going to have attributes. Attributes are analogs to a column in our relational database.
Edges - In relational database we need to create joins to connect tables similer to that we have edges to create connections.These are defined when you create your schema while loading your data.So these precomputed relationships are faster as the runtime computaion like the joins in table are not needed.

## Tiger graph-
Tiger graph is a property graph which means these vertices and edges can contains the attributes.
For e.g suppose you have two vertices payment and order having attributes -id, amount and id, quantity these can have a relation using "accepted" edge which can have a date as attribute.  

## GSQL Commands - 
GSQL is a query language for the graph database.

### Create vertex-
CREATE VERTEX PERSON (PRIMARY_ID ID STRING, email STRING, username STRING, created_at DATETIME) WITH primary_id_as_attribute='true'

### Create directed edge-
CREATE DIRECTED EDGE posted (fROM PERSON To Post, post_date DATETIME) WITH REVERSE EDGE = "reverse_posted"

