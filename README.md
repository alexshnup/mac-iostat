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

*iostat 1*:

```
                   disk0                                          cpu      load average
     r/s   w/s   KB/t  tps     msps     Rmsps     Wmsps    Load us sy id   1m   5m   15m
    0.14   0.44  59.08  10     2662     1166     4292      5.8   1  0 98  1.47 1.42 1.37
    0.00   0.00   0.00   0        0        0        0      0.0   1  1 98  1.47 1.42 1.37
    0.00   0.00   0.00   0        0        0        0      0.0   1  1 97  1.47 1.42 1.37
    0.00   0.00   0.00   0        0        0        0      0.0   5  4 91  1.47 1.42 1.37
    0.02 294.43 941.37 320     2896     1464     2914     91.9  16 16 69  1.47 1.42 1.37
    0.09 370.20 896.86 423     2452    11764     2319     87.5  22 15 63  1.51 1.43 1.37
    0.32 362.71 897.12 414     2401     1230     2424     87.6  16 16 68  1.51 1.43 1.37
    0.27 250.86 828.55 310     3799      894     3895     80.9  11 11 78  1.51 1.43 1.37
    0.14   6.98 609.33  12   315046   363069   280743     59.5  13  5 82  1.51 1.43 1.37
    0.31   2.99 377.33   9   147221    83065   227416     36.8  13  4 83  1.51 1.43 1.37
   17.30   3.08  29.21 714    11188    11487     2931      2.8   9  3 88  1.55 1.44 1.38
   13.24   2.96  61.00 272      657      243     4752      6.0  26  2 71  1.55 1.44 1.38

```


