# Errors

## Disk UNAVAIL
### Problem
After reboot, one Disk is UNAVAIL with a missing or invalid label.
```
  pool: tank
 state: DEGRADED
status: One or more devices could not be used because the label is missing or
        invalid.  Sufficient replicas exist for the pool to continue
        functioning in a degraded state.
action: Replace the device using 'zpool replace'.
   see: http://zfsonlinux.org/msg/ZFS-8000-4J
  scan: scrub in progress since Mon Oct 12 11:04:42 2020
    5.08T scanned out of 9.82T at 69.0M/s, 19h59m to go
    0 repaired, 51.78% done
config:

        NAME                      STATE     READ WRITE CKSUM
        tank                      DEGRADED     0     0     1
          raidz1-0                DEGRADED     0     0     2
            sdb                   ONLINE       0     0     0
            sdc                   ONLINE      27     0     0
            replacing-2           DEGRADED     0     0     0
              old                 OFFLINE      0     0     0
              sda                 ONLINE       0     0     0
            sdd                   ONLINE       0     0     0
            14919388400828854004  UNAVAIL      0     0     0  was /dev/sde1
        logs
          nvme0n1p1               ONLINE       0     0     0
        cache
          nvme0n1p2               ONLINE       0     0     0

errors: No known data errors
```
### Solution
- https://zfsonlinux.org/msg/ZFS-8000-4J/
- https://serverfault.com/questions/656073/zfs-pool-reports-a-missing-device-but-it-is-not-missing
- https://bbs.archlinux.org/viewtopic.php?id=216053

Try reboot first!
** No solution yet **

