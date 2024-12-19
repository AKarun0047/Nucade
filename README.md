# 🚀 **Nessus Report Downloader** 🛡️

Welcome to the **Nessus Report Downloader**! This Python script helps you automate the process of downloading and filtering Nessus scan reports in CSV format. Whether you're a penetration tester, security analyst, or anyone who uses Nessus for vulnerability scanning, this tool will save you time by streamlining the report retrieval and data processing.

---

## 🛠️ **Features**:

- **💼 List Nessus Folders**: Fetch and display all available folders in your Nessus instance.
- **📋 List Scans**: View and select scans within a folder for export.
- **📦 Export Scan Reports**: Automatically export scan results in CSV format with specific columns such as `CVE`, `Hostname`, `Port`, `Solution`, and `CVSS`.
- **⬇️ Download Reports**: Progress bar for downloading reports in real-time.
- **🔄 Retry Mechanism**: The script automatically retries failed HTTP requests for reliable operation.
- **📝 Filter CSV Files**: Clean and filter CSV files to retain only the essential vulnerability data.
- **⚡ Multi-Threaded Downloads**: Efficiently download multiple scan reports in parallel to save time.
- **🔑 Secure API Key Management**: Support for Nessus API keys (use environment variables for added security).

---

## 🎯 **Installation & Setup**:

To get started with this tool, follow the steps below:

### 1. **Clone the Repository**
Clone the repository to your local machine using Git:


git clone https://github.com/<your-username>/nessus-report-downloader.git

---

###2. Install Dependencies

Ensure you have Python 3.x installed, then install the required Python libraries using pip:

cd nessus-report-downloader
pip install -r requirements.txt

###3. Set Your Nessus API Keys

You'll need your Nessus API accessKey and secretKey. It's recommended to store them in environment variables for security:

export NESSUS_ACCESS_KEY="your_access_key"
export NESSUS_SECRET_KEY="your_secret_key"

Alternatively, you can modify the script to directly insert your keys (not recommended for production).
📖 Usage:

    Run the script:

    python nessus_report_downloader.py

    Select a Folder: Once you run the script, it will display a list of available folders in your Nessus instance. Select a folder by number.

    Choose Scans: After selecting a folder, you'll be given the option to either:
        Download all scans in the folder, or
        Download a specific scan by selecting it from the list.

    Download & Filter: The script will export the selected scan(s) as CSV, download them with a progress bar, and filter the CSV file to retain only the essential columns.

###⚙️ Customization Options:

    You can easily modify the columns to filter in the filter_csv() function.
    To customize the report export format, update the payload in the export_scan_to_csv() function.

###🔒 Security:

For enhanced security, avoid hardcoding your Nessus API keys in the script. Instead, use environment variables as shown earlier. This will help protect your keys from exposure, especially when sharing the code.

###🧑‍💻 Contributing:

Feel free to fork this repo and contribute! If you have any bug fixes, suggestions, or improvements, please create a pull request. We'd love to hear from you!


If you have any questions or issues, feel free to open an issue in the GitHub repository.
###👏 Acknowledgments:

    Special thanks to Nessus for providing the powerful vulnerability scanning tool.
    Thanks to requests and pandas for being essential libraries in this script.
    Thanks to colorama for bringing color to the terminal!

###🖼️ Screenshot:

Here’s a sneak peek of how the script looks in action! 👇

Enjoy the automation! 🎉

Disclaimer: This tool is intended to be used only in authorized environments. Please ensure you have the proper permissions before interacting with any Nessus instance.


### Key Highlights in the README:

- **Colorful headings and emojis** to catch attention.
- **Step-by-step installation guide** with commands for easy setup.
- **Feature breakdown** with clear and concise bullet points to explain the script's functionality.
- **Usage instructions** to guide users on how to interact with the script, along with options and expected behavior.
- **Security best practices** regarding API key management, recommending the use of environment variables.
- **Contributing section** to encourage collaboration.
- **License and acknowledgment** sections to give credit to the libraries used and the tool itself.
- **Screenshot** (you can add an actual screenshot or replace the placeholder URL with one from your local machine).

Feel free to adjust the content as needed. The goal is to make the repository stand
