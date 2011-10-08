prototypes
==========

About
-----

This directory contains the EAGLE source files used to manufacture the GAMBY 
prototype boards. These are here for reference only; the final designs 
improve upon there.


Pin Changes
-----------

Several pins were changed between Prototype 1 and Prototype 2. The new pinout
is expected to be the final version. The GAMBY libraries will be written to use
the new pins; if you are one of the few with a Prototype 1 board you will need
to modify the code or the board itself.


+---------------+-------+-------+
|   Function    |  old  |  new  |
+===============+=======+=======+
| LCD SID       |    8  |    8  |
+---------------+-------+-------+
| LCD SCK       |    9  |   10  |
+---------------+-------+-------+
| LCD RS        |   10  |   11  |
+---------------+-------+-------+
| LCD RESET     |   11  |   12  |
+---------------+-------+-------+
| LCD CS        |   12  |   13  |
+---------------+-------+-------+
+---------------+-------+-------+
| B1/Up         |    7  |    7  |
+---------------+-------+-------+
| B2/Left       |    5  |    6  |
+---------------+-------+-------+
| B3/Right      |    4  |    5  |
+---------------+-------+-------+
| B4/Down       |    2  |    4  |
+---------------+-------+-------+
+---------------+-------+-------+
| Audio         |    3  |    9  |
+---------------+-------+-------+
