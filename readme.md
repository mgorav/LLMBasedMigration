# Enhanced Teradata to Databricks Converter

## Overview
This Jupyter notebook is designed to facilitate the conversion of complex Teradata PL/SQL scripts, typically used in SAP data pipelines, into Python code executable within a Databricks environment. The conversion process leverages an open-source large language model for initial code generation, followed by manual refinements to ensure accuracy and efficiency.

Link to nootebook can be found [here](https://colab.research.google.com/github/mgorav/LLMBasedMigration/blob/main/Enhanced_Teradata_to_Databricks_Converter.ipynb)

## Features
- **Automatic Code Conversion**: Utilizes advanced language models to convert Teradata PL/SQL scripts into Python code.
- **Manual Refinement Support**: Provides a framework for further manual adjustments to the automatically generated code.

## Technical Details

### Libraries Used
- `transformers`: For accessing the pre-trained large language model.
- `sqlparse` (optional): For formatting SQL code for improved readability.

### Language Model
The notebook employs open-source models like GPT-Neo or GPT-J from Hugging Face's transformers library. These models are crucial for the initial phase of code conversion.

## Business Value
This tool significantly reduces the time and effort required to convert complex SQL scripts into Python for use in Databricks, accelerating the migration process from Teradata to Databricks. It enhances productivity and reduces the likelihood of manual errors during the conversion process.

## ML Model Justification
- **Why GPT-Neo/GPT-J?**: These models are known for their ability to understand and generate human-like text. Their capability in code generation and natural language understanding makes them ideal for this conversion task.
- **Mathematical Explanation**: These models use a transformer-based architecture, benefiting from self-attention mechanisms to understand the context and dependencies in the input text (PL/SQL scripts) for accurate code generation.

## Steps for Improvement and Pre-training
1. **Data Collection**: Gather a comprehensive dataset of PL/SQL and corresponding Python scripts for Databricks.
2. **Model Pre-training**: Use the collected dataset to fine-tune the language model, enhancing its understanding of PL/SQL and Python syntax and semantics.
3. **Evaluation and Iteration**: Regularly evaluate the model's performance and iterate the pre-training process with new data to continually improve accuracy.
4. **Incorporate User Feedback**: Implement a feedback mechanism to learn from user corrections and integrate this knowledge into subsequent training phases.

## Getting Started
1. Install necessary libraries as mentioned in the "Libraries Used" section.
2. Load the language model using the code provided in the notebook.
3. Input your Teradata PL/SQL script and run the conversion process.
4. Manually refine the output as necessary.

