## <a name='column'> Columnar Databases

Columnar storage and column-oriented query engine are critical to analytical workloads, e.g. OLAP. It's been almost 15 years since it first came out (the MonetDB paper in 1999), and almost every commercial warehouse database has a columnar engine by now.

* [C-Store: A Column-oriented DBMS](http://www.cs.berkeley.edu/~rxin/db-papers/C-Store.pdf) (2005) and [The Vertica Analytic Database: C-Store 7 Years Later](http://vldb.org/pvldb/vol5/p1790_andrewlamb_vldb2012.pdf) (2012): C-Store is an influential, academic system done by the folks in New England. Vertica is the commercial incarnation of C-Store.

* [Column-Stores vs. Row-Stores: How Different Are They Really?](http://db.csail.mit.edu/projects/cstore/abadi-sigmod08.pdf) (2012): Discusses the importance of both the columnar storage and the query engine.

* [Dremel: Interactive Analysis of Web-Scale Datasets](http://research.google.com/pubs/pub36632.html) (2010): A jaw-dropping paper when Google published it. Dremel is a massively parallel analytical database used at Google for ad-hoc queries. The system runs on thousands of nodes to process terabytes of data in seconds. It applies columnar storage to complex, nested data structures. The paper talks a lot about the nested data structure support, and is a bit light on the details of the query execution. Note that a number of open source projects are claiming they are building "Dremel". The Dremel system achieves low-latency through massive parallelism and columnar storage, so the model doesn't necessarily make sense outside Google since very few companies in the world can afford thousands of nodes for ad-hoc queries.
