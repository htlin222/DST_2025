# Load Progress and Backup Steps

## Clone the Repository

```sh
git clone https://github.com/htlin222/DST_2025
```

## Identify Local Data Path

Locate your local data in:

```
$HOME/Documents/Klei/DoNotStarveTogether/xxxxxxxxx/Cluster_xxx
```

## Sync Local Data to Repository

Use `rsync` to back up the folder to the cloned repository:

```sh
rsync -av --progress "/Users/htlin/Documents/Klei/DoNotStarveTogether/437631395/Cluster_1" ~/DST_2025/
```

## Update Cluster Name

Modify the following files:

### 1. `cluster.ini`

- Line 12:

```ini
cluster_name = YOURNAME
```

### 2. `Caves/save/shardindex`

- Line 172:

```ini
name="YOURNAME",
```

### 3. `Master/save/shardindex`

- Line 172:

```ini
name="YOURNAME",
