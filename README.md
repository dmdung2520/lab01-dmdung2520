# Study Assistant — starter

A starter repository for the CSC10014 Smart Virtual Assistant project.

## Setup

Prerequisites: Python 3.10+, Git.
 git clone git@github.com:dmdung2520/lab01-starter.git
 cd lab01-starter
 python -m venv .venv
 source .venv\Scripts\Activate.ps1
 pip install -r requirements.txt
 pip install -e .



## Run

python -m assistant "where is the library?"
 # -> Library: room B.201, open Mon-Sat 07:00-20:00

## Test

pytest -q

## Project structure

- `src/`: Chứa mã nguồn chính của ứng dụng (application code).
- `tests/`: Chứa các kịch bản kiểm thử tự động (automated tests).
- `docs/`: Chứa tài liệu dự án, báo cáo, nhật ký làm việc (logbook).
- `data/`: Chứa các file dữ liệu mẫu với kích thước nhỏ.
- `ui/`: Chứa mã nguồn giao diện người dùng.

## Troubleshooting
- "No module named assistant" -> you forgot `pip install -e .` or the venv is not active.
- PowerShell blocks Activate.ps1 -> Set-ExecutionPolicy -Scope CurrentUser RemoteSigned