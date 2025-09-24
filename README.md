# 🎵 MP3 Reader and Editor

## 📌 Project Overview

This project is a *C-based MP3 metadata editor* that allows you to
*read, validate, and update ID3 tags* (like Title, Artist, Album,
Year, and Comment) in .mp3 files.\
It demonstrates **file handling, error checking, and data manipulation
in C**, making it a great project for embedded systems and systems
programming learners.

---

## 🚀 Features

- ✅ Reads MP3 metadata (tags).\
- ✅ Supports editing the following fields:
  - -t → Title\
  - -a → Artist\
  - -A → Album\
  - -y → Year (validated, must be 4-digit)\
  - -c → Comment\
- ✅ Preserves original audio content after editing.\
- ✅ Handles invalid input gracefully (invalid year, wrong file type,
  missing arguments, etc.).\
- ✅ Works directly with .mp3 files without external libraries.

---

## 🛠 Tech Stack

- *Language:* C\
- *Compiler:* GCC / XC8 (Microchip)\
- *Platform:* Works on Linux/Windows\
- *Concepts Used:* File handling, endian conversion, error handling,
  memory management

---

## ⚙ Usage

### 🏗 Compilation

bash
gcc edit.c mp3.c -o mp3_editor


### ▶ Running the Program

bash
./mp3_editor <option> <new_value> <file.mp3>


### 📖 Examples

bash
./mp3_editor -t "New Song Title" sample.mp3
./mp3_editor -a "Gangadhar" sample.mp3
./mp3_editor -y 2024 sample.mp3


---

## 📂 Project Structure

    ├── edit.c        # Core logic for MP3 editing
    ├── mp3.c         # Helper functions
    ├── mp3.h         # Header file
    ├── sample.mp3    # Example file for testing
    └── README.md     # Project documentation

---

## 🧩 How It Works

1.  *Input Validation* -- Ensures correct tag and .mp3 file.\
2.  *Copy Header* -- Reads MP3 header into a new file.\
3.  *Edit Tag* -- Replaces the specified tag with new content.\
4.  *Copy Remaining Data* -- Preserves original audio content.\
5.  *Replace Old File* -- Removes old file and renames updated file.

---

## SAMPLE OUTPUT
<img width="1283" height="628" alt="Screenshot 2025-09-24 183520" src="https://github.com/user-attachments/assets/e9d690aa-3ddb-44bd-8093-4b452a54134e" />
<img width="1486" height="522" alt="Screenshot 2025-09-24 183642" src="https://github.com/user-attachments/assets/12c11d1f-5e77-4bb6-aadd-2db3545051ac" />

<img width="1497" height="588" alt="Screenshot 2025-09-24 183854" src="https://github.com/user-attachments/assets/9a9f76cf-8b56-40f4-9233-127f8490fe48" />
<img width="1637" height="854" alt="Screenshot 2025-09-24 184229" src="https://github.com/user-attachments/assets/cfd0dde6-0657-43fd-bc48-647f84519a64" />

---
## PROJECT OUPUT DEMO VIDEO
- 🔗 https://drive.google.com/file/d/13JH1ybjDDFEJJy6IEfzD59NUi9ooM5mC/view?usp=sharing
---
## 🛡 Error Handling

- ❌ Invalid year (not 4-digit)\
- ❌ Wrong file type (non-MP3)\
- ❌ Missing arguments\
- ❌ Memory allocation failure\
- ❌ File read/write issues

---

## 🎯 Learning Outcomes

- Hands-on practice with *file handling in C*\
- Understanding *endianness conversion*\
- Implementing *robust error handling*\
- Real-world application: *metadata editing in audio files*

---

## 📌 Future Improvements

- Support for more ID3 tags (genre, track number, lyrics, etc.)\
- GUI interface for easier use\
- Batch editing for multiple MP3 files\
- Cross-platform builds

---

## 👨‍💻 Author

*G Gangadhar*\

- 🔗 Linkedin : https://www.linkedin.com/in/gangadhar-guruginzakunta
  
