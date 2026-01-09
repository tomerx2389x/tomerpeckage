# Custom Colab Utilities

This is your personal Python library for Google Colab.

## How to use in Google Colab

### Option 1: Install from GitHub (Recommended)
1. Upload this folder to a GitHub repository.
2. In your Google Colab notebook, run the following command in a cell:

```python
!pip install git+https://github.com/YOUR_USERNAME/colab_utils.git
```

### Option 2: Install from Local (if uploading the folder to Drive)
If you upload this folder to your Google Drive, mount Drive and install it:

```python
from google.colab import drive
drive.mount('/content/drive')

!pip install -e /content/drive/MyDrive/path/to/colab_utils
```

## Usage

```python
import colab_utils

colab_utils.hello_colab()
```

## Adding new features
1. Add your functions/classes to `colab_utils/core.py` (or create new files).
2. Export them in `colab_utils/__init__.py`.
3. If you add new libraries (like pandas), add them to `install_requires` in `setup.py`.
