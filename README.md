# 🤖 Question Generation using NLP

This project focuses on the automatic generation of different types of educational questions from a given text using **Natural Language Processing (NLP)** techniques. It leverages state-of-the-art language models and NLP libraries to generate **False Statements**, **Fill-in-the-Blank questions**, and **Multiple-Choice Questions (MCQs)** from context or passages.

![Demo](assets/question-generation-demo.gif) <!-- Replace this with your actual GIF file -->

---

## 📌 Overview

The goal of this project is to help automate the manual task of creating educational content for exams, assessments, and learning platforms. It takes in contextual text or statements and generates:

1. **False Statement Generation**  
   From a given true sentence, the model generates false versions by:
   - Splitting the sentence
   - Completing the altered parts using a **GPT-2** language model
   - Introducing misleading context or wording

2. **Fill-in-the-Blanks Question Generation**  
   - Extracts key phrases and concepts from a passage using the **PKE (Python Keyword Extraction)** library
   - Replaces the key terms with blanks
   - Displays the questions in HTML format for better readability

3. **Text-to-MCQ Question Generation**  
   - Summarizes and paraphrases the text using the **T5 Transformer**
   - Generates multiple-choice questions from the summary
   - Creates distractors using **Sense2Vec** to find semantically similar but incorrect alternatives

---

## ✨ Features

- 🧠 Automates educational question creation
- 💬 Uses powerful language models like **GPT-2** and **T5**
- 📚 Handles different question types (True/False, Fill-in-the-Blanks, MCQs)
- ✅ Clean output formatting for web integration
- 🔍 Utilizes NLP techniques such as parsing, summarization, and keyword extraction

---

## 🧠 Algorithms & Techniques

### 🔸 False Statement Generation
- **Constituency Parsing** using **AllenNLP**
- **Sentence Splitting and Completion** using **GPT-2**
- Logical negation and contextual manipulation

### 🔸 Fill-in-the-Blanks Generation
- **PKE Library** for keyword extraction
- **FlashText** for fast keyword replacement
- Cloze-style formatting using HTML templates

### 🔸 Text-to-MCQ Generation
- **T5 Transformers** for summarization and masking
- **Masked Language Modeling** for MCQ stem creation
- **Sense2Vec** for generating semantically relevant distractors

---


---

## 🧰 Tech Stack

| Category            | Tools / Libraries                                |
|---------------------|---------------------------------------------------|
| **Programming**     | Python                                             |
| **NLP Frameworks**  | HuggingFace Transformers, AllenNLP, GPT-2, T5      |
| **Keyword Extraction** | PKE, FlashText                                 |
| **Semantic Similarity** | Sense2Vec                                     |
| **Visualization**   | HTML templates, Jupyter Notebook                  |

---

## 📂 Project Structure

```bash
question-generator-nlp/
│
├── data/                     # Sample input texts and question datasets
├── outputs/                  # Generated questions and HTML files
├── src/                      # Core scripts for each module
│   ├── false_statement_gen.py
│   ├── fill_in_the_blanks.py
│   └── mcq_generator.py
├── assets/                   # Demo GIFs and images
├── requirements.txt
└── README.md


