```sh
lsblk --nodeps --output NAME,ROTA
```

Examine the output of the ROTA column.

* 0 indicates the disk is an SSD (not rotational).
* 1 indicates the disk is an HDD (rotational).

Or checking the rotational file

```sh
cat /sys/block/sdX/queue/rotational
```

Replace `sdX` with the correct disk identifier.

* 0 indicates an SSD
* 1 indicates an HDD
