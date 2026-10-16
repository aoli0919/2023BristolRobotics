# Texture Exploration: Early Dissertation Materials

This repository preserves early dissertation materials for a human single-finger texture exploration project: camera and force-sensor collection scripts, 400 raw force CSVs, and 400 videos from 40 session folders.

For documented data analysis, installation instructions, and the configurable collection software, start with [Human-Texture-Exploration-Experiment](https://github.com/aoli0919/Human-Texture-Exploration-Experiment). That repository is the maintained entry point for this work. Its analysis uses supplied processed data; it does not establish reproduction of the original raw-force or video-to-speed processing, or a paper's results.

## What is preserved here

| Historical material | Location in this repository | Corresponding maintained location |
| --- | --- | --- |
| Original collection entry point | [1.Settings/Main_process.py](1.Settings/Main_process.py) | [Original script](https://github.com/aoli0919/Human-Texture-Exploration-Experiment/blob/main/legacy/acquisition/main.py), [configurable collection software](https://github.com/aoli0919/Human-Texture-Exploration-Experiment/tree/main/acquisition) |
| Original sensor interface | [1.Settings/forcesensor.py](1.Settings/forcesensor.py) | [Original interface](https://github.com/aoli0919/Human-Texture-Exploration-Experiment/blob/main/legacy/acquisition/forcesensor.py), [collection guide](https://github.com/aoli0919/Human-Texture-Exploration-Experiment/blob/main/docs/acquisition.md) |
| Raw force CSVs and videos | [2.Raw_dataset/](2.Raw_dataset/) | [Force CSVs](https://github.com/aoli0919/Human-Texture-Exploration-Experiment/tree/main/data/raw/force), [videos](https://github.com/aoli0919/Human-Texture-Exploration-Experiment/tree/main/data/raw/video) |

A Git blob comparison found all 800 raw-data files byte-for-byte identical to those in the original Human repository, under different paths. They are shared source material, rather than an additional dataset. The two scripts here are earlier versions and are not the current runnable collection software.

The historical scripts require a compatible camera, FT300-series force sensor, serial connection, GUI, and external Python dependencies. They contain fixed device and output settings and have no hardware-free mode. Their presence does not establish that collection can run on a new machine; hardware operation has not been validated as part of this documentation update. Use the maintained repository's collection guide and dry-run entry point to prepare a new session.

See [provenance](docs/provenance.md) for the comparison, original path mappings, and verification scope. The [original README](docs/original-readme.md) is retained unchanged as a historical record; its result statements and citation placeholder are not validation or publication metadata.
