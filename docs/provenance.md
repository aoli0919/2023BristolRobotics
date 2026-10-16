# Provenance and repository relationship

This repository is an early dissertation-project record. [Human-Texture-Exploration-Experiment](https://github.com/aoli0919/Human-Texture-Exploration-Experiment) is the maintained entry point for documented analysis and collection software.

## Comparison basis

On 16 October 2026, the complete recursive Git tree of this repository at commit [`5d6daca1d9018b9cef3e7ef511804ddcaa309bc3`](https://github.com/aoli0919/2023BristolRobotics/tree/5d6daca1d9018b9cef3e7ef511804ddcaa309bc3) was compared with the original Human repository's saved Git blob manifest, before its directory reorganization. The tree was not truncated. The comparison used blob SHA values and paths, without downloading the large data blobs.

| Comparison | Result |
| --- | --- |
| Historical Bristol files | 803 blobs |
| Raw-data files with identical blob SHA in Human | 800: 400 CSVs and 400 MP4s |
| Total bytes of those matching raw-data files | 619,995,159 |
| Matching files at the same path | 0; all 800 use different directory paths |
| Remaining files | README and two collection scripts; 19,120 bytes in total |

Identical Git blob SHA values establish identical file bytes. They do not validate measurement units, synchronization, processing algorithms, statistical conclusions, or reproduction of a publication. The Human repository also holds processed workbooks, questionnaire material, and documentation absent from this historical tree.

## Path mapping

`<session>` and `<N>` below denote the existing session-folder names and trial numbers.

| Bristol path, retained here | Original Human path | Current Human path |
| --- | --- | --- |
| `2.Raw_dataset/<session>/force_data_<N>.csv` | `Raw Data/Raw_Force/<session>/force_data_<N>.csv` | [`data/raw/force/`](https://github.com/aoli0919/Human-Texture-Exploration-Experiment/tree/main/data/raw/force)`<session>/force_data_<N>.csv` |
| `2.Raw_dataset/<session>/video_<N>.mp4` | `Raw Data/Raw_Video/<session>/video_<N>.mp4` | [`data/raw/video/`](https://github.com/aoli0919/Human-Texture-Exploration-Experiment/tree/main/data/raw/video)`<session>/video_<N>.mp4` |
| [`1.Settings/Main_process.py`](../1.Settings/Main_process.py) | `Processing Code/main.py` | [`legacy/acquisition/main.py`](https://github.com/aoli0919/Human-Texture-Exploration-Experiment/blob/main/legacy/acquisition/main.py) |
| [`1.Settings/forcesensor.py`](../1.Settings/forcesensor.py) | `Processing Code/forcesensor.py` | [`legacy/acquisition/forcesensor.py`](https://github.com/aoli0919/Human-Texture-Exploration-Experiment/blob/main/legacy/acquisition/forcesensor.py) |

The two Bristol scripts have different blob SHA values from their Human counterparts. Source comparison shows earlier collection implementations with differences in comments, prompts, formatting, device defaults, and implementation details. This is historical source provenance, not evidence of a separate analysis pipeline. The current configurable implementation is in [`acquisition/`](https://github.com/aoli0919/Human-Texture-Exploration-Experiment/tree/main/acquisition); see its [guide](https://github.com/aoli0919/Human-Texture-Exploration-Experiment/blob/main/docs/acquisition.md).

## Preservation and verification

This update changes only the landing documentation and adds this provenance note and an exact copy of the previous [README](original-readme.md). All 802 other original file paths and blob SHA values remain unchanged, including both collection scripts and all raw data. No data are moved, deleted, or regenerated.

The two historical Python files were parsed for syntax. Their dependencies, GUI, camera, serial interface, sensor operation, and physical timing were not tested. The maintained repository documents a hardware-free collection dry run and processed-data analysis; those capabilities do not retroactively validate the historical scripts or the original acquisition hardware.
