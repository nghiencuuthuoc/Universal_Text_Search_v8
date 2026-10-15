# Universal Text Search v8 — PharmApp

Tìm nội dung chữ bên trong Excel, Word, PDF, HTML và văn bản thuần (SQLite FTS5, không cần gõ dấu).
Search inside Excel, Word, PDF, HTML and plain-text files (SQLite FTS5, accent-insensitive).

PySide6 / Qt 6.9 · Windows / macOS / Linux · 5 themes: System, Light, Dark, Luxury Warm, Modern Blue-Gray.

## Run / Chạy

```bash
pip install -r requirements.txt
python run.py                         # modular package in app/
python Universal_Text_Search_v8.py    # single-file edition
```

Windows: `Universal_Text_Search_v8.bat` (finds portable `Python312`, installs PySide6 if missing).
A ready-built exe (~23 MB) is in `dist/Universal_Text_Search_v8.exe`.

## Build the smallest exe / Build exe nhỏ nhất

```bat
build_exe.bat
```

Uses a clean venv + PyInstaller, only QtCore/QtGui/QtWidgets, optional UPX
(put `upx.exe` in `tools/upx/`; it is not committed).

## Tests

```bash
pytest -q
```

## Documentation / Tài liệu

Bilingual SOP (VI/EN) in `docs/`: `.docx`, `.pdf`, `.xlsx`, `.html`, `.pptx`.
Regenerate with `python tools/sop/build_sop.py` (edit `tools/sop/content.py`).

## Layout

```
app/        main window, theme/, widgets/, models/, dialogs/, core/ (index, extractors, workers), utils/
tests/      pytest suite
tools/      make_single_file.py, sop/ (SOP generators)
assets/     nct_logo.png, nct_logo.ico
docs/       SOP files
```

© 2009-2026 • Pharma R&D Platforms • PharmApp • [www.nghiencuuthuoc.com](https://www.nghiencuuthuoc.com) •
[Zalo: +84888999311](https://zalo.me/84888999311) • [www.pharmapp.dev](https://www.pharmapp.dev)
