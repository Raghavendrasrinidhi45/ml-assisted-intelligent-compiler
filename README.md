# ML-Assisted Intelligent Compiler for Automated Syntax Error Detection and Recovery

## Overview
This educational prototype demonstrates lexical analysis, recursive-descent syntax analysis, syntax-error classification, diagnostic suggestions, and panic-mode recovery for a small C-like language.

## Requirements
- Python 3.10+
- Optional: `pip install -r requirements.txt` for the small TF-IDF/Logistic Regression demonstration. The program also runs without scikit-learn using rule-based labels.

## Run
From this folder:
```bash
python src/compiler.py
```

## Supported language subset
- Declarations: `int total = 10;`
- Assignments: `total = total + 5;`
- Output: `print(total);`
- Return: `return total;`
- Arithmetic expressions with `+`, `-`, `*` is only partially implemented: the demo parser handles `+` and `-`; parentheses and identifiers/numbers are supported.

## Project structure
- `src/compiler.py`: complete prototype source
- `tests/test_compiler.py`: unit tests
- `outputs/sample_output.txt`: captured demonstration output
- `main.tex`: Overleaf-ready report using the supplied report's general layout (A4, 12pt, Times, one-inch margins, numbered sections, code listings, references)

## Important academic note
The ML component is a small illustrative classifier trained on synthetic examples, not a production-trained model. The test/output data are demonstrative and should be described as such. Replace student names/IDs and supervisor details before submission.
