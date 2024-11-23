The Codon Optimizer V 3.0/
│
├── README.md                     # Overview of the project (details from your markdown)
├── LICENSE                       # License file (MIT License)
├── requirements.txt              # List of dependencies
├── .gitignore                    # Ignored files and folders
├── data/                         # Folder for input and example data files
│   └── example_sequences.xlsx    # Example input file for DNA sequences
├── src/                          # Source code directory
│   ├── __init__.py               # Makes src a package
│   ├── data_loader.py            # Functions for loading data
│   ├── preprocessing.py          # Preprocessing utilities for mutation and tokenization
│   ├── model.py                  # Transformer model definition
│   ├── embeddings.py             # Functions for ESM embeddings
│   ├── beam_search.py            # Beam search decoder implementation
│   ├── gui.py                    # GUI code using tkinter
│   └── main.py                   # Main entry point to run the pipeline
├── notebooks/                    # Jupyter Notebooks for experiments and examples
│   └── example_workflow.ipynb    # Demonstrates project workflow
├── tests/                        # Unit tests for the project
│   ├── __init__.py               # Makes tests a package
│   ├── test_data_loader.py       # Tests for data loader
│   ├── test_preprocessing.py     # Tests for preprocessing functions
│   ├── test_model.py             # Tests for the model
│   ├── test_embeddings.py        # Tests for embeddings functionality
│   └── test_gui.py               # Tests for the GUI
└── docs/                         # Documentation for the project
    ├── overview.md               # Detailed overview of the project
    ├── usage.md                  # Usage instructions
    ├── features.md               # Explanation of features
    └── future_work.md            # Notes on future enhancements
