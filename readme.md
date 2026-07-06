# Nepali Audio To Text
- This is a system capable of generating Nepali transcripts for the Nepali speech input. This system uses the Nepali ASR model [wav2vec2-nepali](https://huggingface.co/anish-shilpakar/wav2vec2-nepali) which is a fine-tuned version of Facebook's wav2vec2 model for Nepali dataset
- This system is a small part of [SwarSaransha](https://github.com/JuJu2181/Automatic-Nepali-Speech-Recognition-and-Summarizer)
- **Developed By:** [Anish Shilpakar](https://github.com/JuJu2181)
- Web Interface for this system will be created soon. Stay tuned.

## Steps to configure this system
### 1. Clone this repository
```
https://github.com/JuJu2181/NepaliAudio2Text
```
### 2. Install FFMPEG
As, we are dealing with various audio formats in this project, FFmpeg is essential for succesfull running of this project. So I kindly request you to install a suitable version of FFmpeg in your computer before running this project.
You can download FFmpeg from this link [FFMPEG](https://ffmpeg.org/download.html)

### 3. Install requirements.txt  
- First use uv to create a virtual environment with python version 3.12 and then install these requirements
```
uv venv --python 3.12
source .venv/bin/activate
```
If you haven't installed uv you can install it using this [uv installation](https://docs.astral.sh/uv/getting-started/installation/#pypi)

Then install the requirements
```
uv pip install -r requirements.txt
```

### 4. Create a temp directory
Before you run the project, manually create a temp directory in the project's root directory
```
mkdir temp
```

### 5. Run the project
```
python audio_to_text.py
```

## Output:
Here you have 2 options either to convert all the audio files in a folder to their transcripts or simply convert a single audio file to its transcript. And the output for both these modes are shown below:
### 1. Generating Transcript for Folder of Audio files
![Folder Output](screenshots/output_folder.png)
### 2. Generating Transcript for a single audio file
![File Output](screenshots/output_file.png)
