# NetBSD-Fujitsu-S700
Kernel configuration for optimization of Fujitsu Futro S700

> Warning! License may change due to lack of header in GENERIC configuration from syssrc.tgz file

## Long term goals:
 - Smaller file size of NetBSD kernel
 - Lower CPU usage
 - Lower memory usage
 - Disable everything that is not needed
 - Build kernel for NetBSD 9.0 (Currently 8.1, then patch)
 
## Repository files:
| Filename    | Description                                           |
| :---:       | :---:                                                 |
|README.md    |Readme file                                            |
|dmesg-GENERIC|`dmesg` output on GENERIC kernel                       |
|dmesg-DEBUG  |`dmesg` output on current modified kernel configuration|
|S700KERNCONF |Modified kernel configuration file                     |

## Flags in configuration:
| Flag   | Description                               |
| :---:  | :---:                                     |
|MODIFYME|Option which is user dependent             |
|CHECKME |Check if changing this value boots properly|

## Differences:
|                   | GENERIC  | S700KERNCONF |
| :---:             | :---:    | :---:        |
| Size (bytes)      | 24880560 | 12601504     |
| Boot time (sec)   |          |              |
| Mem. Load (bytes) |          |              |


## Resources:
 - [how to reduce kernel size - NetBSD wiki](https://wiki.netbsd.org/tutorials/how_to_reduce_kernel_size/)
 - [tuning netbsd for performance - NetBSD wiki](https://wiki.netbsd.org/tutorials/tuning_netbsd_for_performance/)
 - [Chapter 19. Tuning NetBSD - NetBSD Guide](https://www.netbsd.org/docs/guide/en/chap-tuning.html)

### Misc
 - [NetBSD sources (8.1)](http://cdn.netbsd.org/pub/NetBSD/NetBSD-8.1/source/sets/)
 
