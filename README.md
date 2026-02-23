#  Mashup Predictive Analysis – YouTube Mashup Generator

An interactive Streamlit-based web application that automatically creates an audio mashup from multiple YouTube videos of a selected singer and delivers it directly to the user's email.

This project fulfills the requirements of the Mashup Programming Assignment, including both a Command-Line utility and a Web-based interface.

---

##  Project Highlights

✔ Automated YouTube video downloading  
✔ Audio extraction and smart trimming  
✔ Mashup generation from multiple clips  
✔ ZIP packaging of final output  
✔ Direct email delivery to user  
✔ Secure credential storage using Streamlit Secrets  
✔ Automatic cleanup of temporary files  

---

##  Application Preview

![Application UI](UI.png)

---

##  System Workflow

### Step 1 – User Inputs
-  Singer Name  
-  Number of videos (must be greater than 10)  
-  Duration per video (more than 20 seconds)  
-  Valid email address  

### Step 2 – Backend Processing
- Searches and downloads videos using `yt-dlp`
- Extracts audio using `FFmpeg`
- Trims first *Y* seconds from each file
- Combines all clips into a single mashup
- Compresses output into `mashup.zip`
- Sends the ZIP file via email
- Deletes temporary files after completion

---

## 🛠 Technology Stack

| Technology | Purpose |
|------------|----------|
| Python | Core Programming |
| Streamlit | Web Interface |
| yt-dlp | YouTube Downloading |
| FFmpeg | Audio Processing |
| SMTP (Gmail App Password) | Email Delivery |

---

##  Security Configuration

Sensitive email credentials are stored using **Streamlit Secrets**.

Create the following file locally:
<img width="847" height="90" alt="image" src="https://github.com/user-attachments/assets/0bc7d069-707a-41f9-81a6-4c507e5f9f3e" />

## 📦Requirements

Create a file named `requirements.txt` and add:
<img width="841" height="85" alt="image" src="https://github.com/user-attachments/assets/dfe25f30-18d0-4709-ac68-09d4241ab03b" />

## Assignment Implementation Details

This project satisfies the requirements of both the command-line based program and the web-based application as described in the assignment.

### 1. Command Line Application

The CLI program includes:

- Proper validation of input parameters  
- Structured exception handling to manage runtime errors  
- Extraction, trimming, and merging of audio files  
- Generation of a compressed ZIP archive containing the final mashup  

### 2. Web-Based Application

The Streamlit web application provides:

- An interactive and user-friendly interface  
- Validation of user inputs before processing  
- Automated email delivery of the generated mashup  
- Secure handling of credentials using Streamlit Secrets  

---

## Author

Gurvani Ahuja


