Here’s a **clean, simple, fully English README** version for your project, with a neutral technical tone and no emojis.

---

# unblurrit

**unblurrit** is a lightweight Python tool for deblurring and enhancing photos using **OpenCV**.
It supports multiple image enhancement methods and can process single images or entire folders.

## Features

* Unsharp Masking for professional image sharpening
* CLAHE (Contrast Limited Adaptive Histogram Equalization) for detail enhancement
* Wiener Deconvolution for motion blur reduction
* Batch processing for directories
* Simple command-line interface

---

## Repository

```bash
git clone https://github.com/libertates/unblurrit.git
cd unblurrit
```

---

## Virtual Environment

```bash
python3 -m venv .venv
source .venv/bin/activate  # macOS / Linux
```

---

## Installation

```bash
pip install opencv-python numpy
```

---

## Usage

### Single Image

```bash
python deblur.py my_photo.jpg
```

### Directory (Batch Processing)

```bash
python deblur.py images/
```

---

## Method Selection

You can explicitly choose the enhancement method using the `-m` flag:

```bash
python deblur.py image1.jpg -m unsharp
python deblur.py image1.jpg -m combined
```

### Available Methods

* `basic` – quick sharpening
* `unsharp` – unsharp masking
* `wiener` – Wiener deconvolution (motion blur)
* `enhance` – detail enhancement (CLAHE)
* `combined` – combination of multiple methods

---

## Requirements

* Python 3.8+
* OpenCV
* NumPy
