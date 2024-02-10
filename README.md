# File-Downloads-Automator


**Description:**

This Python script automates the organization of your downloaded files, neatly sorting them into designated folders based on their type (audio, video, image, document, or a special SFX category). It continuously monitors a specified download directory and moves new files to the appropriate locations, keeping your download folder tidy and saving you time.

**Key Features:**

- **Automatic file organization:** Eliminates manual sorting of downloaded files.
- **Customizable categories:** Define specific folders for audio, video, images, documents, and SFX to match your workflow.
- **Cross-platform compatibility:** Works seamlessly on Windows, macOS, and Linux.
- **Efficient and resource-friendly:** Lightweight script with minimal impact on your system.
- **User-friendly:** Clear and concise instructions for setup and usage.

**How to Use:**

**1. Installation:**

- Clone or download this repository to your local machine.
- Ensure you have Python 3.6 or later installed on your system. You can check this by running `python3 --version` in your terminal. If you don't have it, download it from [https://www.python.org/downloads/](https://www.python.org/downloads/).

**2. Configuration:**

- Open the `file_downloads_automaton.py` script in a text editor.
- Locate the following variables and update them with your desired paths:

  ```python
  # Replace with your desired download directory
  source_dir = "C:/Users/Username/Downloads"

  # Customize folder paths for file types
  dest_dir_sfx = "C:/Downloads/SFX"
  dest_dir_music = "C:/Downloads/Music"
  dest_dir_video = "C:/Downloads/Videos"
  dest_dir_image = "C:/Downloads/Images"
  dest_dir_documents = "C:/Downloads/Documents"
  ```

- **Note:** Replace `"Username"` with your actual username and adjust the paths according to your system's directory structure.

**3. Running the Script:**

- Open a terminal or command prompt and navigate to the directory where you saved the script.
- Run the script using the following command:

  ```bash
  python file_downloads_automaton.py
  ```

- The script will start monitoring your download directory and automatically move new files to the appropriate folders.

**4. Optional: Setting Up Automatic Execution (Windows)**

- Create a `.bat` file named `start_script.bat` in the same directory as the script.
- Add the following line to the `start_script.bat` file:

  ```
  python file_downloads_automaton.py
  ```

- You can now double-click this `start_script.bat` file to launch the script, or schedule it to run automatically using Task Scheduler.

**Customization:**

- You can modify the supported file extensions for each category in the script based on your preferences.
- The script uses logging to track its activity. You can enable logging by uncommenting the line `logging.basicConfig(...)` in the script.

**Troubleshooting:**

- If you encounter any issues, consult the comments within the script and search online for solutions related to Python file handling and the `watchdog` library.