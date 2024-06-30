# Speech Recognizer

## Overview
This Speech Recognizer is a Python-based tool that transcribes audio files into text. It uses advanced audio processing techniques and the SpeechRecognition library to accurately convert speech to text.

## Features
- Transcribes WAV audio files to text
- Handles large audio files by splitting them into manageable chunks
- Utilizes silence detection for improved accuracy

## Prerequisites
Before you begin, ensure you have met the following requirements:
- Python 3.6 or higher
- FFmpeg (for audio file conversion)

## Installation

1. Clone this repository:
2. Install the required Python packages:
    Ensure FFmpeg is installed on your system. If not, install it:
- On Ubuntu or Debian: `sudo apt-get install ffmpeg`
- On macOS with Homebrew: `brew install ffmpeg`
- For Windows, download from the [official FFmpeg website](https://ffmpeg.org/download.html)

## Usage

1. Convert your audio file to WAV format (if it's not already):
2.  Run the speech recognition script:
3.  When prompted, enter the path to your WAV file.

4. The script will process the audio and output the transcribed text.

## Configuration

You can adjust the following parameters in the script for better performance:
- `min_silence_len`: Minimum length of silence (in milliseconds) that will be used to split the audio
- `silence_thresh`: The threshold (in dBFS) below which to consider as silence
- `keep_silence`: Amount of silence to keep around each chunk

## Troubleshooting

- If you encounter a "FileNotFoundError", ensure that the audio file path is correct and the file exists.
- For "AudioSegment" related errors, make sure you have FFmpeg installed and accessible in your system PATH.

## Contributing

Contributions to this project are welcome. Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [SpeechRecognition library](https://pypi.org/project/SpeechRecognition/)
- [Pydub library](https://github.com/jiaaro/pydub)
