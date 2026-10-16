# Python Programming: IIST Training for CAPF and IB Officials

Course material for the **Python Programming** training programme run by the Department of Avionics, Indian Institute of Space Science and Technology (IIST), Thiruvananthapuram, from **28 September to 10 October 2026**, for officials of SSB, CRPF, BSF and IB.

The course takes a beginner from first programs to a working project: Python fundamentals, data structures and functions, files, NumPy and Pandas, cleaning and analysing data, visualization and images, and a final project presentation.

## What is in this repository

The same material is organised in two ways, so you can take what you need.

| Folder | What it holds | Use it when |
|---|---|---|
| [`combined/`](combined/) | One notebook (`.ipynb`) and one slide deck (`.pptx`) covering the whole course in schedule order | You want everything in one place |
| [`individual/`](individual/) | All 28 original files, one folder per schedule day, unchanged | You want one specific lecture, lab or notebook |
| [`datasets/`](datasets/) | The CSV files used by the notebooks | You are running a notebook yourself |

## Repository pattern

```
python-programming-iist-2026/
├── README.md                  this file
├── combined/
│   ├── README.md
│   ├── Python_Programming_Complete_Notebook.ipynb
│   └── Python_Programming_Complete_Slides.pptx
├── individual/
│   ├── README.md
│   ├── Day01_Introduction_and_Setup/
│   ├── Day02_Python_Fundamentals_I/
│   ├── Day03_Python_Fundamentals_II/
│   ├── Day04_Data_Structures_and_Functions/
│   ├── Day05_Project_Discussion/
│   ├── Day06_Environments_and_Files/
│   ├── Day07_NumPy_and_Pandas/
│   ├── Day08_Data_Cleaning_and_Analysis/
│   ├── Day09_Visualization_and_Images/
│   ├── Day10_Project_Presentations/
│   └── Supplementary_Not_in_Schedule/
└── datasets/
    ├── README.md
    ├── fifa_data.csv
    ├── gas_prices.csv
    └── tips.csv
```

Each Day folder holds its own `README.md` (schedule slot, file list, notes) plus the slides and notebooks used that day. Day folders are numbered to match the course schedule, and the same Day, Session order is used inside the combined notebook and the combined slides.

## Schedule and where to find each day

| Day | Date (2026) | Topics | Folder | Files |
|---|---|---|---|---|
| Day 1 | 28 September 2026 | Inauguration, Introduction to Computing and Python Setup | [Day01_Introduction_and_Setup](individual/Day01_Introduction_and_Setup/) | 1 |
| Day 2 | 29 September 2026 | Python Fundamentals I; Input, Output and Basic Programming | [Day02_Python_Fundamentals_I](individual/Day02_Python_Fundamentals_I/) | 3 |
| Day 3 | 30 September 2026 | Python Fundamentals II; Loops and Repetition | [Day03_Python_Fundamentals_II](individual/Day03_Python_Fundamentals_II/) | 2 |
| Day 4 | 1 October 2026 | Data Structures in Python; Functions and Modular Programming | [Day04_Data_Structures_and_Functions](individual/Day04_Data_Structures_and_Functions/) | 5 |
| Day 5 | 2 October 2026 | Project Discussion and Doubt Clarification | [Day05_Project_Discussion](individual/Day05_Project_Discussion/) | 0 |
| Day 6 | 5 October 2026 | Python Environment and Libraries; File and Folder Management | [Day06_Environments_and_Files](individual/Day06_Environments_and_Files/) | 1 |
| Day 7 | 6 October 2026 | Introduction to Data Processing (NumPy); Pandas and Tabular Data | [Day07_NumPy_and_Pandas](individual/Day07_NumPy_and_Pandas/) | 2 |
| Day 8 | 7 October 2026 | Data Cleaning and Filtering; Data Analysis with Pandas | [Day08_Data_Cleaning_and_Analysis](individual/Day08_Data_Cleaning_and_Analysis/) | 3 |
| Day 9 | 8 October 2026 | Data Visualization and Multimodal Data; Working with Images | [Day09_Visualization_and_Images](individual/Day09_Visualization_and_Images/) | 7 |
| Day 10 | 9 October 2026 | Doubt Clearing, Project Guidance and Student Project Presentations | [Day10_Project_Presentations](individual/Day10_Project_Presentations/) | 0 |

Day 11 (Saturday 10 October) was the valedictory and closing day and has no teaching material.

## How to use the material

1. **Get the files.** Click the green **Code** button, then **Download ZIP**, or clone the repository with `git clone`.
2. **Set up Python.** Follow `individual/Day01_Introduction_and_Setup/Anaconda_Conda_Jupyter_Project_Setup_Guide.pdf` to create a Conda environment and register it as a Jupyter kernel.
3. **Install the libraries** the notebooks use: `numpy`, `pandas`, `matplotlib`, `seaborn`, `pillow`, `jupyter`.
4. **Open a notebook** in Jupyter and run it one section at a time. Keep the folder layout as it is, because the combined notebook reads data from `../datasets/`.
5. **Study in schedule order**, or jump to one day from the table above.

## Known issues in the original material

These were found while preparing the repository. The original files were left unchanged.

- **Day 3, `Class_Python_Fundamentals_II.ipynb`:** one starter cell in the menu-driven converter has `{value * LITRE_TO_GALLON.4f}`, which needs a colon (`:.4f`), or the cell raises a SyntaxError.
- **Day 9, `Matplotlib_Tutorial_FIFA_and_Gas_Prices.ipynb`:** two cells use `.count()[0]`, which fails on current pandas. Use `.count().iloc[0]` instead.
- **Material not in the source folder:** Day 1 introduction slides, Day 3 theory slides, and the Day 6 and Day 7 lab notebooks. The Day 5 and Day 10 sessions had no slides or notebooks.
- **Day 8 slides** are the second half of the Pandas deck stored in the Day 7 folder.

## Original file names

The files were renamed to describe their content. This table gives each original file name and its place in the repository.

| Original file name | Location in this repository |
|---|---|
| `Anaconda_Conda_Jupyter_Project_Setup_Guide.pdf` | [`individual/Day01_Introduction_and_Setup/Anaconda_Conda_Jupyter_Project_Setup_Guide.pdf`](individual/Day01_Introduction_and_Setup/Anaconda_Conda_Jupyter_Project_Setup_Guide.pdf) |
| `DAY 2_DIYA.pdf` | [`individual/Day02_Python_Fundamentals_I/Day2_Session1_Python_Fundamentals_Slides.pdf`](individual/Day02_Python_Fundamentals_I/Day2_Session1_Python_Fundamentals_Slides.pdf) |
| `day_2.pdf` | [`individual/Day02_Python_Fundamentals_I/Day2_Session2_Input_Output_Basic_Programming_Slides.pdf`](individual/Day02_Python_Fundamentals_I/Day2_Session2_Input_Output_Basic_Programming_Slides.pdf) |
| `day2_practice_questions.pdf` | [`individual/Day02_Python_Fundamentals_I/Day2_Practice_Questions.pdf`](individual/Day02_Python_Fundamentals_I/Day2_Practice_Questions.pdf) |
| `Class_Python_Fundamentals_II(1).ipynb` | [`individual/Day03_Python_Fundamentals_II/Class_Python_Fundamentals_II.ipynb`](individual/Day03_Python_Fundamentals_II/Class_Python_Fundamentals_II.ipynb) |
| `Class_Python_Fundamentals_II.ipynb` | [`individual/Day03_Python_Fundamentals_II/Class_Python_Fundamentals_II_earlier_version.ipynb`](individual/Day03_Python_Fundamentals_II/Class_Python_Fundamentals_II_earlier_version.ipynb) |
| `Prateek_Data_Structures_in_Python.pptx` | [`individual/Day04_Data_Structures_and_Functions/Data_Structures_in_Python_Slides.pptx`](individual/Day04_Data_Structures_and_Functions/Data_Structures_in_Python_Slides.pptx) |
| `Neeraj_Theory_Functions_and_Modular_Programming-1.pptx` | [`individual/Day04_Data_Structures_and_Functions/Functions_and_Modular_Programming_Slides.pptx`](individual/Day04_Data_Structures_and_Functions/Functions_and_Modular_Programming_Slides.pptx) |
| `Neeraj_Lab_Functions_Student.ipynb` | [`individual/Day04_Data_Structures_and_Functions/Lab_Functions_Student.ipynb`](individual/Day04_Data_Structures_and_Functions/Lab_Functions_Student.ipynb) |
| `Neeraj_Lab_Functions_Instructor_Solutions.ipynb` | [`individual/Day04_Data_Structures_and_Functions/Lab_Functions_Instructor_Solutions.ipynb`](individual/Day04_Data_Structures_and_Functions/Lab_Functions_Instructor_Solutions.ipynb) |
| `python_class.pdf` | [`individual/Day04_Data_Structures_and_Functions/Python_Classes_Objects_and_Methods_Slides.pdf`](individual/Day04_Data_Structures_and_Functions/Python_Classes_Objects_and_Methods_Slides.pdf) |
| `Python_Environments_Libraries_and_Files.pdf` | [`individual/Day06_Environments_and_Files/Python_Environments_Libraries_and_Files_Slides.pdf`](individual/Day06_Environments_and_Files/Python_Environments_Libraries_and_Files_Slides.pdf) |
| `numpy_lecture.pdf` | [`individual/Day07_NumPy_and_Pandas/NumPy_Lecture_Slides.pdf`](individual/Day07_NumPy_and_Pandas/NumPy_Lecture_Slides.pdf) |
| `Data_Cleaning_Pandas (2).pptx` | [`individual/Day07_NumPy_and_Pandas/Pandas_Data_Processing_Slides.pptx`](individual/Day07_NumPy_and_Pandas/Pandas_Data_Processing_Slides.pptx) |
| `Data_Cleaning_Pandas_Demo.ipynb` | [`individual/Day08_Data_Cleaning_and_Analysis/Data_Cleaning_Pandas_Demo.ipynb`](individual/Day08_Data_Cleaning_and_Analysis/Data_Cleaning_Pandas_Demo.ipynb) |
| `Data_Cleaning_Pandas_Exercises.ipynb` | [`individual/Day08_Data_Cleaning_and_Analysis/Data_Cleaning_Pandas_Exercises.ipynb`](individual/Day08_Data_Cleaning_and_Analysis/Data_Cleaning_Pandas_Exercises.ipynb) |
| `Data_Cleaning_Pandas_Solutions.ipynb` | [`individual/Day08_Data_Cleaning_and_Analysis/Data_Cleaning_Pandas_Solutions.ipynb`](individual/Day08_Data_Cleaning_and_Analysis/Data_Cleaning_Pandas_Solutions.ipynb) |
| `Python_Data_Visualization (1).pdf` | [`individual/Day09_Visualization_and_Images/Data_Visualization_and_Multimodal_Data_Slides.pdf`](individual/Day09_Visualization_and_Images/Data_Visualization_and_Multimodal_Data_Slides.pdf) |
| `Matplotlib Tutorial.ipynb` | [`individual/Day09_Visualization_and_Images/Matplotlib_Tutorial_FIFA_and_Gas_Prices.ipynb`](individual/Day09_Visualization_and_Images/Matplotlib_Tutorial_FIFA_and_Gas_Prices.ipynb) |
| `matplotlib_tutorial.ipynb` | [`individual/Day09_Visualization_and_Images/Matplotlib_Tutorial_30_Minutes.ipynb`](individual/Day09_Visualization_and_Images/Matplotlib_Tutorial_30_Minutes.ipynb) |
| `handson_STUDENT.ipynb` | [`individual/Day09_Visualization_and_Images/Hands_on_Data_Visualization_Student.ipynb`](individual/Day09_Visualization_and_Images/Hands_on_Data_Visualization_Student.ipynb) |
| `Pillow_Theory_Slides.pdf` | [`individual/Day09_Visualization_and_Images/Images_Pillow_Theory_Slides.pdf`](individual/Day09_Visualization_and_Images/Images_Pillow_Theory_Slides.pdf) |
| `Pillow_Lab_Slides.pdf` | [`individual/Day09_Visualization_and_Images/Images_Pillow_Lab_Slides.pdf`](individual/Day09_Visualization_and_Images/Images_Pillow_Lab_Slides.pdf) |
| `Pillow_Lab_Exercise.ipynb` | [`individual/Day09_Visualization_and_Images/Images_Pillow_Lab_Exercise.ipynb`](individual/Day09_Visualization_and_Images/Images_Pillow_Lab_Exercise.ipynb) |
| `Consolidated_Lab_Sheet.ipynb` | [`individual/Supplementary_Not_in_Schedule/Machine_Learning_Lab_Sheet.ipynb`](individual/Supplementary_Not_in_Schedule/Machine_Learning_Lab_Sheet.ipynb) |
| `fifa_data.csv` | [`datasets/fifa_data.csv`](datasets/fifa_data.csv) |
| `gas_prices.csv` | [`datasets/gas_prices.csv`](datasets/gas_prices.csv) |
| `tips.csv` | [`datasets/tips.csv`](datasets/tips.csv) |

## Credits

Programme organiser and coordinator: Mukhilan Lenin. Programme coordinator: Dr. Deepak Mishra, Department of Avionics, IIST.

Slides and notebooks were prepared by the course instructors. Names are shown only where they were printed on the material itself (for example Diya P M, Dhevamathi C, Ramzan Basheer, Lt. Col. Neeraj Sharma, Prateek Rathore and Mr. Jayakumar T V). Each folder's README says which instructor a file is credited to.

## Licence

No licence has been chosen for this repository. Until one is added, the material is shared for learning use by the programme participants, and the authors keep their rights over their own slides and notebooks.
