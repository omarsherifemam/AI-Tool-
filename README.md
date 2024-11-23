# DNA Sequence Optimization Tool

## Overview
This project provides a comprehensive pipeline to optimize DNA sequences based on protein sequences. It combines cutting-edge machine learning techniques with user-friendly tools to help researchers and biologists optimize DNA sequences efficiently. The primary functionalities include:

- **Mutating DNA Sequences**: Introduces realistic mutations to enhance the robustness of DNA optimization.
- **Protein Translation**: Converts DNA sequences into corresponding protein sequences.
- **Transformer-based Optimization**: Utilizes advanced transformer models to generate optimized DNA sequences tailored to input protein sequences.
- **Interactive GUI**: Offers a graphical interface where users can input protein sequences and obtain optimized DNA sequences with a single click.

This tool is designed for users in molecular biology, bioinformatics, and genetic engineering to streamline DNA optimization workflows. With this tool, you can preprocess DNA data, train custom optimization models, and generate results seamlessly.

## Features
- **Protein-DNA Optimization**: Translate protein sequences into optimized DNA codons.
- **Transformer-based Model**: Custom Transformer layers for sequence learning.
- **Mutation Simulation**: Introduce realistic mutations for training robust models.
- **Pretrained Embeddings**: Use ESM-2 embeddings for protein sequences.
- **GUI Interface**: Interactive GUI for users to input protein sequences and retrieve optimized DNA sequences.

## How to Use

### Step 1: Data Preparation
1. Prepare an Excel file with a column named `Sequence` containing DNA sequences.
2. Save the file in a location accessible by the script.

### Step 2: Running the Code
1. Open the code and locate the `excel_path` variable in the `main()` function.
2. Update the path to point to your Excel file.
3. Run the script using your preferred Python environment.

### Step 3: GUI Interaction
1. Once the GUI is launched, enter a protein sequence into the input text box.
2. Click the **Generate Optimized DNA Sequence** button.
3. The optimized DNA sequence will appear in the output section of the GUI.

## Workflow
1. **Data Loading**: The script reads DNA sequences from an Excel file, validates them, and translates them into protein sequences.
2. **Preprocessing**: Mutations are introduced to the DNA sequences to simulate real-world variability. Sequences are tokenized and padded for model training.
3. **Model Training**: The transformer-based model is trained or fine-tuned for DNA sequence optimization.
4. **GUI**: Users interact with an intuitive interface to input protein sequences and obtain optimized DNA sequences.

## Time Breakdown
The development of this tool was completed in **16 hours**, divided as follows:

- **Data Loading and Preprocessing (4 hours)**:
  - Writing functions to load data from Excel files.
  - Implementing mutation simulation and sequence tokenization.
- **Model Implementation (5 hours)**:
  - Building the transformer-based DNA optimization model.
  - Integrating pretrained embeddings from ESM-2.
- **GUI Development (3 hours)**:
  - Creating an interactive interface using `tkinter`.
  - Ensuring the GUI is intuitive and easy to use.
- **Testing and Debugging (2 hours)**:
  - Validating data processing and optimization results.
  - Ensuring compatibility across different hardware setups.
- **Documentation and Finalization (2 hours)**:
  - Writing the README file and detailed usage instructions.
  - Preparing example files and refining the workflow.

## Key Functions

### Data Loading
```python
load_data(excel_path, sheet_name=0, max_rows=None)
```
- Reads DNA sequences from an Excel file.
- Translates sequences into proteins.

### Preprocessing
- `introduce_realistic_mutations`: Simulates mutations for robust model training.
- `preprocess_sequences`: Tokenizes and prepares DNA and protein sequences.

### Model
- **Custom Transformer Block**: Implements a Transformer layer for sequence optimization.
- `create_model`: Defines and compiles the model.

### GUI
- `create_gui`: Launches a user-friendly GUI to input protein sequences and retrieve optimized DNA.

## Pretrained Components

### ESM-2 Model
- **Source**: [Hugging Face (facebook/esm2_t6_8M_UR50D)](https://huggingface.co/facebook/esm2_t6_8M_UR50D)
- **Usage**: Generates embeddings for protein sequences.

### Transformer Model
- **Custom Implementation**: Decodes DNA sequences using protein embeddings.

## Training the Model

### Preprocessing
- Tokenizes and introduces mutations to DNA sequences.
- Pads sequences to a consistent length.

### Training
- Trains a Transformer-based model.
- Automatically saves the trained model for future use.

## Outputs
- **Optimized DNA Sequence**: The GUI displays the optimized DNA sequence based on user-provided protein sequences.

## Notes
- Use a well-structured Excel file with a `Sequence` column.
- Ensure TensorFlow and PyTorch are installed and GPU support is enabled for faster processing.
- Training the model may take significant time, depending on the dataset and hardware.

## Future Enhancements
- Support for larger protein databases.
- Batch processing through the GUI.
- Enhanced visualization for mutations and optimizations.
