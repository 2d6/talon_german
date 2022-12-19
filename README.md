# Talon German
German Dictation Mode for Talon Voice

## Status
This is the first prototype, don't expect a highly satisfying user experience.

## Dependencies
This is a plug-in for Talon Voice (https://talonvoice.com/).

## Setup
* download the newest German language model from [alphacephei][alphacephei] into `~/.talon/vosk/`:
  ```
  mkdir -p ~/.talon/vosk
  cd ~/.talon/vosk
  curl -LfSo vosk-model-de.zip https://alphacephei.com/vosk/models/vosk-model-de-0.21.zip
  unzip vosk-model-de.zip
  mv vosk-model-de-* vosk-model-de
  ```
* run `~/.talon/bin/pip install vosk` (on windows `%appdata%\talon\.venv\Scripts\pip.bat install vosk`)
* clone this repository into your talon user folder (`~/.talon/user`)

It won't work on mac unless you sign the pip installed library file yourself, or unless aegis ships the vosk kaldi library with talon pre-signed.

## Usage
Say "german" to switch from command mode to German dictation mode and "english/englisch" to switch back. Check out the german.talon and german.py files for German commands.

[alphacephei]: https://alphacephei.com/vosk/models
