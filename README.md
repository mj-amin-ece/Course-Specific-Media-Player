# Course-Specific Media Player

**A PyQt5 video player for recorded lectures. Each session comes with an Excel file of topic tags, and clicking a tag jumps straight to that part of the lecture.**

![Python](https://img.shields.io/badge/Python-3-3776AB?logo=python&logoColor=white)
![PyQt5](https://img.shields.io/badge/GUI-PyQt5-41CD52?logo=qt&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?logo=pandas&logoColor=white)

Final project for the *Advanced Programming* course (Dr. Amir Jahanshahi), Amirkabir University of Technology. Developed by Mohammad Javad Amin and Faeze.

## Features

- **Tag navigation:** load a session's Excel tag file and click any topic to seek to its timestamp.
- **Tag editing:** add or edit tags while you watch, then save the updated tag file anywhere.
- **Playback controls:** play and pause, variable speed, volume, and skipping forward or back.
- **Viewing:** full-screen and zoom, plus several color themes (default, sky, white, dark).
- **Keyboard shortcuts** for seeking and zooming.

A short screen recording is in [`docs/demo.mp4`](docs/demo.mp4), and the full write-up is in [`docs/report.pdf`](docs/report.pdf).

## Repository structure

```text
.
├── app/
│   ├── main.py             # application entry point (VideoWindow)
│   ├── requirements.txt
│   └── image/              # backgrounds and icons
├── sample-tags/            # tag files for the course sessions (session*.xlsx)
└── docs/
    ├── demo.mp4            # usage demo
    └── report.pdf          # project report
```

## Getting started

```bash
cd app                      # icons are loaded relative to this folder
python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python main.py
```

Open a lecture video, then load its tag file from `sample-tags/` to get clickable topics.

## Author

**Mohammad Javad Amin** · [GitHub](https://github.com/mj-amin-ece)
