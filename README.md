# Student Information System — Version 1

A desktop-based Student Information System (SSIS) built with Python and Tkinter, using CSV files for data storage. This is the first version of the system, focusing on core CRUDL functionality for managing students, programs, and colleges.

---

## Tech Stack

| Layer | Technology |
|-------|------------|
| Language | Python |
| GUI Framework | Tkinter |
| Data Storage | CSV Files |

---

## Features

- **Student Management** — Create, Read, Update, Delete, and List student records
- **Program Management** — Manage academic programs (e.g., BSCS, BSIT)
- **College Management** — Manage colleges (e.g., CCS, COE)
- **Search** — Search students by ID, name, course, or other fields
- **Sorting** — Sort records by column
- **Pagination** — Browse through large sets of records efficiently
- **Photo Upload** — Attach a student photo to each record (optional)

---

## Data Structure

### Student (`student_data.csv`)
| Field | Description |
|-------|-------------|
| `id` | Unique student ID in format `YYYY-NNNN` (e.g., 2023-0001) |
| `firstname` | Student's first name |
| `lastname` | Student's last name |
| `course` | Refers to a program code (e.g., BSCS) |
| `year` | Year level |
| `gender` | Gender |
| `photo` | Optional photo of the student |

### Program (`courses.csv`)
| Field | Description |
|-------|-------------|
| `code` | Program code (e.g., BSCS) |
| `name` | Full program name (e.g., Bachelor of Science in Computer Science) |
| `college` | Refers to a college code |

### College (`colleges.csv`)
| Field | Description |
|-------|-------------|
| `code` | College code (e.g., CCS) |
| `name` | Full college name (e.g., College of Computer Studies) |

---

## Getting Started

### Prerequisites
- Python 3.x
- Tkinter (usually bundled with Python)

### Installation & Run

```bash
# Clone the repository
git clone https://github.com/aeron-j/SSIS_V1.git
cd SSIS_V1

# Run the application
python Main/151project.py
```

> No additional dependencies needed — all data is stored locally in CSV files.

---

## Project Structure

```
SSIS_V1/
└── Main/
    ├── 151project.py     # Main entry point — GUI and all logic
    ├── colleges.csv      # College data
    ├── courses.csv       # Program/course data
    ├── student_data.csv  # Student records
    └── student.png       # Default student photo placeholder
```

---

## Notes

- This is **Version 1** — data is stored in flat CSV files, no database used
- See [SSIS_V2](https://github.com/aeron-j/SSIS_V2) for the improved MySQL version
- See [webssis](https://github.com/aeron-j/webssis) for the final web-based version

---

## Author

**Aeron Dale** — [@aeron-j](https://github.com/aeron-j)
