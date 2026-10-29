# University Classroom & Laboratory Timetabling Benchmark Dataset (V7.0)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Benchmark: PATAT/ITC](https://img.shields.io/badge/Benchmark-PATAT--ITC-blue.svg)](https://www.patatconference.org/)
[![Python: 3.8+](https://img.shields.io/badge/Python-3.8%2B-green.svg)](https://www.python.org/)

## 1. Overview & Provenance

This dataset is a standardized benchmark for Automated Classroom and Laboratory Scheduling / Course Timetabling Systems. Adapted from international PATAT (Practice and Theory of Automated Timetabling) and ITC benchmark instances.

## 2. Directory Structure

```
University_Classroom_Timetabling_Dataset/
├── Classroom_Booking_Dataset_V7.xlsx    # Unmodified relational dataset
├── README.md                            # Benchmark documentation
├── LICENSE                              # MIT Open Source License
├── requirements.txt                     # Dependencies
├── config.json                          # Schema configuration
├── scripts/
│   ├── dataset_loader.py
│   ├── conflict_checker.py
│   └── timetable_solver.py
└── benchmarks/
    └── sample_schedules.json
```

## 3. Schema & Rules
- Users (116 records), Classes (242 records), Laboratories (15 records), Schedule (16 records).
- Hard Constraints: Capacity non-violation, no room/faculty double booking.
- Soft Constraints: TWOINAROW (10), TWOINADAY (20), PERIODSPREAD (30), FRONTLOAD (15).
