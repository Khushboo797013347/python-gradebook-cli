Python Mini Project – Gradebook CLI

Overview

Gradebook CLI is a command-line application developed using Python. It manages students, courses, enrollments and grades.



Features

Add students and courses.



Enroll students in courses.



Add and manage grades.



Calculate course averages.



Calculate student GPA.



Store data using JSON files.



Validate user inputs.



Log application activities and errors.



Project Structure

gradebook/

├── data/

│   └── gradebook.json

├── gradebook/

│   ├── \_\_init\_\_.py

│   ├── models.py

│   ├── service.py

│   ├── storage.py

│   └── validation.py

├── logs/

│   └── app.log

├── scripts/

│   └── seed.py

├── tests/

│   └── test\_service.py

├── main.py

├── README.md

└── .gitignore

Setup

Create a virtual environment:



python -m venv venv

Activate it on Windows:



venv\\Scripts\\activate

Run the application

python scripts/seed.py

python main.py --help

Testing

python -m unittest discover -s tests -v

Design Decisions \& Limitations

* Python classes represent students, courses and enrollments.



* JSON is used for simple local data persistence.



* Argparse provides command-line interaction.



* Exception handling helps manage invalid inputs and missing data.



* The application is designed for local use and does not use a database or web interface.



