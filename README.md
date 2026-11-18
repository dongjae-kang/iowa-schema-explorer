# Iowa Schema Explorer

An interactive 3D map of the Iowa Liquor Sales class database. It shows the same data at three levels: the result one query returns, the design behind it, and the four tables PostgreSQL stores.

Live site: https://dongjae-kang.github.io/iowa-schema-explorer/

- Click a result column to trace its value down to the stored row it comes from; click the travelling value to see the join key that brought it there.
- Click a table to zoom in and read real rows; click a join to see which keys find a match and which do not.
- Red cubes are sales rows that an INNER JOIN leaves out (1 cube is about 100 rows).
- Walk the exercise builds the four-table query step by step.
- Zoom with the bar at the top right, or scroll or pinch over the 3D view. A Text version link in the side panel shows the same facts without 3D.
- Dark by default, with a light theme button in the header.

Data: Iowa Alcoholic Beverages Division, published on data.iowa.gov, as distributed in SIPA IA 6652. Every number was measured on a local PostgreSQL copy of the course CSV files (sales 3,049,913 rows, stores 1,973, products 9,977, counties 99).

Built by Dongjae Kang with three.js, with help from AI coding tools (Claude and Codex).
