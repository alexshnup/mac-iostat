mac-iostat
==========

Extended iostat for Mac OS X.

Based on the official version (system_cmds 550.10) of iostat from Apple, this version prints some more detailed information about disk I/O operations. For example it's able to show you seperated values for *written and read megabytes per second*.

How to build:
-------------
```
make all
make install
```

It should be located here:
```
/usr/local/bin/xiostat
```

How to use:
-----------

See 'man iostat'

Example output:
---------------

```
iostat -d disk2 1
                   disk2
     r/s     w/s     KB/t      tps      mspt     Rmspt    Wmspt   util
    0.08     0.10     9.30    19.00     0.23     0.19     0.36    33.93
    0.00     0.00     0.00     0.00     0.00     0.00     0.00     0.00
    0.00     0.00     0.00     0.00     0.00     0.00     0.00     0.00
   16.06     5.47     4.00  5511.26     0.16     0.17     0.15    49.92
   19.10     6.24     4.00  6487.51     0.17     0.17     0.15    74.43
   19.27     6.26     4.00  6535.00     0.17     0.17     0.15    86.93
   18.47     6.21     4.00  6318.19     0.16     0.17     0.15    92.93
    0.00     0.00     0.00     0.00     0.00     0.00     0.00     0.00
    1.99     0.00   410.40     4.98     2.11     2.58     0.19    17.82
    0.00     0.00     0.00     0.00     0.00     0.00     0.00     0.00
```


