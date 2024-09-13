# Audio Processing Script

This script processes audio files by separating stereo channels, applying timestamps, and adjusting the audio properties. It uses the `pydub` library for audio manipulation and `tqdm` for progress tracking.

## Features

- Separates stereo audio files into left and right channels.
- Applies the timestamp of the input file to the output file.
- Adjusts the frame rate and sample width of the audio files.
- Logs the processing steps and outputs to a log file.

## Requirements

- Python 3.x
- `pydub` library
- `tqdm` library

You can install the required libraries using pip:

```bash
pip install pydub tqdm
```

## Usage

To run the script, use the following command:

```bash
python script_name.py <input_dir> <output_dir>
```

- `<input_dir>`: Directory containing the input audio files.
- `<output_dir>`: Directory to store the output files.

## Example

```bash
python audio_processing.py /path/to/input /path/to/output
```

## Functions

### `setup_logging(log_file)`

Sets up logging for the script.

### `apply_file_timestamps(input_file, output_file)`

Applies the timestamp of the input file to the output file.

### `process_files(input_dir, output_dir)`

Processes audio files with timestamp and stereo separation.

### `pan_and_merge(left_channel, right_channel)`

Applies panning to left and right channels and merges them into a stereo track.

## Logging

The script generates a log file in the output directory with the current timestamp. The log file contains detailed information about the processing steps and any errors encountered.
