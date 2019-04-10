# Good parameters
<https://jrs-s.net/2018/08/17/zfs-tuning-cheat-sheet/> seems to work well

for `ashift=12`, set during pool creation, all others, run
```
zfs set property=value <dataset>
```


# Commands to remember

```
zpool create <name> -o ashift 12 <mirror|raidz> /dev/disk/by-id/<diskid>
```

```
zfs list -r -t snapshots <dataset>
```

