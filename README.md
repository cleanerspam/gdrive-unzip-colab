# GDrive Unzip Colab

**GDrive Unzip Colab** is an interactive Google Colab notebook for browsing Google Drive folders, extracting ZIP files safely, and automatically cleaning up verified archives. It is designed for data professionals, researchers, and automation enthusiasts who manage large compressed datasets in Google Drive.

---

## Features

- Interactive Google Drive folder navigation.
- Batch extraction of all `.zip` files in the selected folder.
- Safe verification of extracted files before deleting the original ZIPs.
- Flat extraction structure – all files are placed in a unified `unzipped` folder.
- Persistent log (`unzipped_log.txt`) for progress tracking and resume capability.
- Local SSD-based extraction for faster performance and reduced Drive I/O errors.

---

## Open in Google Colab

Open the notebook directly in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/cleanerspam/gdrive-unzip-colab/raw/refs/heads/main/gdrive_unzip_colab.ipynb)

> Change `USERNAME` with your GitHub username after forking this repo.

---

## Usage

1. Open the notebook in Google Colab using the link above.  
2. Mount your Google Drive when prompted.  
3. Use the interactive folder selector to choose the Drive folder containing ZIP files.  
4. The script will:
   - Extract each ZIP file locally in the Colab environment.
   - Copy the extracted contents into a new `unzipped` folder in the same Drive directory.
   - Delete the original ZIP files only after successful verification.
   - Maintain a log file to track completed extractions.
5. If interrupted, rerun the notebook — previously processed files will be skipped automatically.

---

## Example Workflow

| Step | Action | Result |
|------|---------|--------|
| 1 | Select Drive folder | `/MyDrive/Data/Zipped` |
| 2 | Local extraction in Colab | Faster processing on temporary SSD |
| 3 | Copy to Drive | `/MyDrive/Data/Unzipped` |
| 4 | Verification and cleanup | Original ZIPs deleted after verification |

---

## Requirements

- A Google account with Google Drive access.  
- A Google Colab session (Free, Pro, or Pro+).  
- No external installations required – all dependencies are pre-installed.

---

## Why Use This Notebook

Google Drive does not natively support extracting large ZIP archives.  
This notebook provides a safe, automated, and verifiable way to handle bulk ZIP extraction and cleanup operations without manual downloads or third-party tools.  
It is particularly useful for managing research datasets, project archives, and cloud backups directly within Drive.

---

## Repository Tags

`google-drive` `colab` `automation` `unzip` `data-management` `file-processing`

---

## Contributing

Contributions, issues, and feature requests are welcome.  
Future enhancements may include:
- Multi-folder batch selection.
- Progress bar integration.
- Notification or reporting features.

Please submit pull requests or suggestions via the Issues tab.

---

## License

BSD 3-Clause License © 2025  

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this list of conditions, and the following disclaimer.  
2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions, and the following disclaimer in the documentation and/or other materials provided with the distribution.  
3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
