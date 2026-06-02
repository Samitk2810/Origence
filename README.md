# Origence — NLP-Based Academic Plagiarism Detection System

Origence is a batch-based academic plagiarism detection system designed to ensure document originality within academic institutions. The system enables faculty to create batches, define plagiarism thresholds, and monitor submissions, while students can join batches and upload documents for automated plagiarism checking.

---

## Features

### Faculty Module

* Create batches with unique batch codes
* Configure similarity threshold for each batch
* View all created batches
* Track students enrolled in batches
* Monitor student submissions
* View uploaded documents batch-wise
* Check similarity scores and document status
* Track accepted and rejected submissions

### Student Module

* Register and log in securely
* Join batches using batch codes
* Upload academic documents
* Automatic plagiarism checking before submission
* View submission status and similarity score
* Upload allowed only when similarity is below the defined threshold

---

## NLP-Based Plagiarism Detection

Origence incorporates Natural Language Processing (NLP) techniques to improve document comparison and plagiarism analysis.

### NLP Techniques Used

* Text preprocessing
* Tokenization
* Text normalization
* Stop-word removal
* Similarity analysis
* Batch-wise document comparison

### Detection Workflow

```text
Document Upload
       ↓
Text Extraction
       ↓
NLP Preprocessing
       ↓
Similarity Analysis
       ↓
Threshold Validation
       ↓
Accepted / Rejected
```

---

## Core Logic

Each uploaded document is compared only with documents belonging to the same batch.

### Decision Rules

```text
If Similarity Score < Threshold
       → Accepted

If Similarity Score ≥ Threshold
       → Rejected
```

The similarity threshold is configured by faculty members and dynamically applied during document validation.

---

## System Architecture

```text
Faculty / Student
        ↓
      Batch
        ↓
Document Upload
        ↓
NLP Processing
        ↓
Similarity Analysis
        ↓
Threshold Validation
        ↓
Accepted / Rejected
```

---

## Tech Stack

### Frontend

* Flutter
* Dart

### Backend

* Django
* Python
* REST APIs

### Database

* SQLite

### Concepts Used

* Natural Language Processing (NLP)
* Similarity Analysis
* Role-Based Access Control
* Batch Management System

---

## Project Structure

```text
origence/
│
├── frontend/
├── backend/
│   ├── api/
│   ├── auth_api/
│   ├── core/
│   ├── db.sqlite3
│   └── manage.py
│
├── docs/
│
└── README.md
```

---

## Authentication System

* Username and Password based authentication
* Secure login mechanism
* Role-based authorization

### Supported Roles

* Faculty
* Student

---

## Database Design

### Main Entities

* User
* Batch
* Batch Membership
* Document

### Document Attributes

* Student Information
* Batch Information
* Uploaded File
* Similarity Score
* Acceptance Status
* Upload Timestamp

---

## Key Highlights

* NLP-powered plagiarism detection
* Batch-specific document comparison
* Dynamic threshold control
* Faculty monitoring dashboard
* Role-based access management
* Automated acceptance and rejection workflow
* Scalable architecture for academic institutions

---

## Future Enhancements

* AI-based semantic similarity detection
* PDF plagiarism highlighting
* Cross-batch plagiarism comparison
* Admin dashboard
* Cloud deployment (AWS/Firebase)
* Email and in-app notifications
* Advanced analytics and reporting

---

## Contribution

This project was developed as a collaborative academic project. Contributions, suggestions, and improvements are welcome.

---

## Authors

* Arhat Jadhav
* Samit Kadam

---

## License

This project is intended for educational and academic purposes.

---

## Final Note

Origence provides an efficient and scalable solution for academic plagiarism detection by combining batch-based document management with NLP-driven similarity analysis, helping educational institutions maintain academic integrity.
