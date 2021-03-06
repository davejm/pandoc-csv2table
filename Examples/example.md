---
title: CSV to Pandoc Markdown Tables
author: Wasif Baig
date: May 08, 2015
---

All tables in this document have been generated by post-processing through
[pandoc-csv2table-filter][filter].


Simple Table
------------

You can include inline markdown in your csv file.
It will be parsed by the pandoc markdown reader.
You can also specify column alignments in the [configuration string][config].

![A **simple** _table_. sycr](csv/simple.csv)


Multiline Table
---------------

It allows cell contents to span multiple lines, unlike simple table.

![A **_`multiline`_** table. mccr](csv/multiline.csv)


Grid Table
----------

It lets you inlcude block markdown as well, unlike multiline tables.
However, it does not support column alignments.
Every column is default-aligned.

![A sample Grid Table. gycccccc](csv/grid.csv)

Pipe Table
----------

It is like a simple table feature-wise.

![Demonstration of pipe table syntax. prldc](csv/pipe.csv)

Final Words
-----------

You only need either a *multiline* table or a *grid table*.
**Multiline** tables allow control over column alignments.
**Grid** tables allow inclusion of block level elements.

License
-------

[pandoc-csv2table-filter][filter] 

The MIT License

Copyright © 2015 Wasif Hasan Baig <pr.wasif@gmail.com>

Acknowledgements
----------------

Thanks to [John MacFarlane][john] for creating [Pandoc][pandoc].


[john]: http://johnmacfarlane.net/
[pandoc]: http://pandoc.org/
[filter]: https://github.com/baig/pandoc-csv2table-filter
[config]: https://github.com/baig/pandoc-csv2table-filter#configuration-string