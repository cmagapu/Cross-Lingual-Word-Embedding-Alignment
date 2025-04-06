# Cross-Lingual-Word-Embedding-Alignment
Implementing and evaluating a supervised cross-lingual word embedding alignment system for English and Hindi using the Procrustes method.

---

## Instructions to Run the Notebook

This project implements both **supervised** and **unsupervised** cross-lingual word embedding alignment for English–Hindi, using the Procrustes method and adversarial training with CSLS (based on the MUSE framework).

---

### Requirements

Install dependencies using pip:

```bash
pip install fasttext torch numpy scipy matplotlib
```

> **Note for Mac M1/M2/M3 (Apple Silicon):**  
> You may need to install the CPU-only version of PyTorch:

```bash
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cpu
```

---

### Files & Folder Structure

The notebook will automatically download the following files if not present:

- `cc.en.300.bin` — pre-trained English FastText embeddings  
- `cc.hi.300.bin` — pre-trained Hindi FastText embeddings  
- `en-hi.txt` / `hi-en.txt` — MUSE bilingual dictionaries

```
project_directory/
├── notebook.ipynb             # Main notebook (run this)
├── cc.en.300.bin              # (downloaded automatically)
├── cc.hi.300.bin              # (downloaded automatically)
├── en-hi.txt / hi-en.txt      # (downloaded automatically)
```

If you're running offline, make sure these files are already in the directory.

---

### Running the Notebook

1. Open a terminal in the project directory.
2. Launch Jupyter Notebook:

```bash
jupyter notebook
```

3. Open `notebook.ipynb` and run all cells in order.

---

### Optional: Create Conda Environment

```bash
conda create -n xling-align python=3.10
conda activate xling-align
pip install fasttext torch numpy scipy matplotlib
```
