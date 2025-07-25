# DMS (Document Management System)

A simple Flask-based document management system for uploading, searching, previewing, and managing documents.

## Features
- User login (admin/user)
- Upload PDF, DOCX, TXT, DOC files
- Add explanation for each document
- Search and filter by filename and date
- Preview PDF, TXT, and DOCX files in browser
- Admins can delete files (with deleted by info)
- Tracks who uploaded and deleted each file

## Usage
1. Install dependencies:
   ```bash
   pip install flask werkzeug python-docx
   ```
2. Run the app:
   ```bash
   python app.py
   ```
3. Open [http://localhost:5000](http://localhost:5000) in your browser.

## Login Credentials
- **Admin:**  
  Username: `admin`  
  Password: `adminpass`
- **User:**  
  Username: `user`  
  Password: `userpass`

## File Storage
- Uploaded files are stored in the `uploads/` folder.
- Metadata (uploader, explanation, deleted by) is stored in `uploads/metadata.json`.

## Notes
- Only admins can delete files.
- Users can only view and download/preview files.
- Explanations are optional and shown in the file list.

---
Simple, extensible, and ready for your organization!
