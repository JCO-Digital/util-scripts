# util-scripts

A collection of utility scripts for server management and other things.

## Scripts

### `link-bin`

A utility to create a symbolic link for a script in `/usr/local/bin` and make it executable. This allows you to run your scripts from anywhere.

**Usage:**

```bash
sudo ./link-bin <script_name>
```

### `server-restart`

Schedules a server restart at a specified time (defaults to 01:00). It also runs `apt update && apt upgrade` before the restart unless skipped.

**Usage:**

```bash
./server-restart [time] [--skip-update] [--help]
```

**Options:**

- `[time]`: The time to restart the server (default: 01:00).
- `--skip-update`: Skip running `apt update` and `apt upgrade`.
- `--help`: Show the help message.
