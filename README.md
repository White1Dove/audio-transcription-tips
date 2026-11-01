# Audio transcription tips

A short, practical list for anyone turning recordings into text: developers, researchers, podcasters and students.

## Free and local
- **OpenAI Whisper**: open-source speech recognition you run yourself. `pip install -U openai-whisper`, then `whisper file.mp3 --model small`.
- **whisper.cpp**: a fast C/C++ port that runs well on laptops without a GPU.
- **ffmpeg**: extract the audio from a video first if a tool only accepts audio: `ffmpeg -i video.mp4 -vn -acodec copy audio.m4a`.

## Online
- Look for speaker labels, timestamps and SRT export. Check the free limits before uploading a long file.
- Disclosure: I built Transcribe Audio, a tool for [audio transcription with speaker labels](https://transcribeaudio.co). Files up to 30 minutes are free.

## Getting a better transcript
- Record close to the speaker; distance hurts more than noise.
- One person speaking at a time keeps speaker labels clean.
- Set the language manually if the file starts with music or silence.
- Always proofread names, numbers and quotes.

## Formats
| Format | Use it for |
|---|---|
| TXT | Search, notes, LLM summaries |
| DOCX | Editing and sharing |
| SRT / VTT | Subtitles and captions |

Contributions welcome: open a pull request with a tool or tip you rely on.
