# YouTube Transcriber and Word Cloud Generator

This project is a Python-based tool designed to:

1. Download audio from YouTube videos.
2. Transcribe the audio using the AssemblyAI API.
3. Generate a word cloud from the transcription.
4. Integrate with Excel for user inputs and outputs using `xlwings`.
5. Run the Python script directly from a button in the Excel interface and display the process in designated cells.

## Features

- **YouTube Audio Downloader**: Extracts and converts YouTube videos to MP3 audio files.
- **Audio Transcription**: Uploads audio to AssemblyAI and retrieves a transcription.
- **Word Cloud Generator**: Creates a graphical word cloud representation of the transcription.
- **Excel Integration**: Uses an Excel spreadsheet as a simple user interface.
- **Excel Macro Integration**: Runs the Python script directly from a button in Excel.

## Requirements

### Python Libraries

Ensure the following Python libraries are installed:

- `requests`
- `xlwings`
- `pytube`
- `wordcloud`

Install them using:
```bash
pip install requests xlwings pytube wordcloud
```

### Additional Requirements

- Microsoft Excel (for `xlwings` and macro integration).

## Files

- **`transcriber1.py`**: Main Python script.
- **`transcriber1.xlsm`**: Excel file for user interaction and macro execution.

## Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/sahilgoyal7214/VocalTranscriber
   cd VocalTranscriber
   ```

2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Open the Excel file (`transcriber1.xlsm`). The following features are pre-configured:
   - A button to run the Python script.
   - Cells for entering inputs:
     - `YOUTUBE_URL`: Enter the YouTube video URL.
     - `API_KEY`: Provide your AssemblyAI API key.
     - `TRANSCRIBE`: Set to `True` to enable transcription.
     - `WORDCLOUD`: Set to `True` to generate a word cloud.
     - `STATUS_CELL`: Displays the current status of the process.
     - `TITLE_CELL`: Displays the YouTube video title.

4. Use the button in the Excel interface to trigger the Python script. The process and results will be displayed in the designated cells.

## Usage

1. Enter the required data in the Excel file.
2. Click the button in the Excel file to trigger the script.
3. Outputs:
   - Transcribed text will be saved as a `.txt` file in the project directory.
   - Word cloud will be saved as a `.png` file in the project directory.

## Limitations

- Requires an active internet connection for downloading videos and interacting with AssemblyAI.
- Processes one video at a time.





## Contributing

Contributions are always welcome!

See `contributing.md` for ways to get started.




## Authors

- [Sahil Goyal](https://www.github.com/sahilgoyal7214)

