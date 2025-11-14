# Huron

A package registry index for some released projects maintained with [Orbit](https://github.com/chaseruskin/orbit).

## Configuration

To access the configurations and get the most out of these settings, you should at least have `git` installed and found on your system's PATH.

1. Download the profile from its remote repository using `git`:
```
git clone https://github.com/hyperspace-labs/huron.git "$(orbit env ORBIT_HOME)/channels/huron"
```

2. Link the channel in the home configuration using `orbit`:
```
orbit config --push include="channels/huron/config.toml"
```

## Usage

To view available projects from Huron (and potentially any other configured channels), run:
```
orbit search --available
```

To get more insight into a particular project, run:
```
orbit info <project>
```

To install a particular project, run:
```
orbit install <project>
```

## Synchronization

To pull the latest available versions and projects from Huron (and potentially any other configured channels), run:
```
orbit --sync
```