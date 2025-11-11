# legal-bert-based-contract-analyzer

An AI-powered tool that automatically detects and extracts important clauses from legal contracts using **Legal-BERT** (a transformer model fine-tuned on the **CUAD dataset**).

## Overview
Contracts contain dozens of clauses that require careful review.  
This project leverages **Natural Language Processing (NLP)** and **Transformer-based models** to automatically identify key legal clauses such as:

- Governing Law  
- Effective Date  
- Termination  
- Confidentiality  
- Limitation of Liability  
- Indemnity  
- Audit Rights  
- Assignment  
- Notice  

The model classifies sentences into multiple legal clause categories and highlights only the **important sentences**, making contract review faster and more efficient.

##  Model Performance

| Metric | Score |
|:--|:--|
| **Validation Loss** | 0.157 |
| **Macro F1-Score** | 0.988 |
| **Micro F1-Score** | 0.992 |
| **Subset Accuracy** | 0.480 |
| **Epochs** | 5 |
| **Base Model** | `nlpaueb/legal-bert-base-uncased` |

 **High precision and recall**  
 **Excellent generalization**  
 **No overfitting observed**

 ##  Dataset — CUAD (Contract Understanding Atticus Dataset)

- Contains over **510 commercial contracts**
- Annotated for **41 clause categories**
- Developed by **The Atticus Project**
- Used for fine-tuning Legal-BERT on clause classification tasks  
- [CUAD Dataset on Hugging Face](https://huggingface.co/datasets/theatticusproject/cuad)


##  Technologies Used
- **Python 3.10+**
- **Transformers (Hugging Face)**
- **PyTorch**
- **Scikit-learn**
- **Pandas / NumPy**
- **Gradio** (for Web UI)
- **PyPDF2** and **python-docx** (for reading documents)


##  Features
- Detects and classifies **41 types of legal clauses**
- Highlights only **important and relevant sentences**
- Works with `.pdf`, `.docx`, and `.txt` files
- Displays results in an **interactive Gradio dashboard**
- Outputs predictions and JSON summaries for downstream use



input  document
<img width="998" height="675" alt="image" src="https://github.com/user-attachments/assets/c86976b6-7911-4f84-93a9-05f608feb9f1" />

output 
<img width="876" height="476" alt="image" src="https://github.com/user-attachments/assets/2ba2bbea-6c43-4287-9de1-4b3369727497" />
<img width="882" height="378" alt="image" src="https://github.com/user-attachments/assets/7983de0c-f6d5-45e0-b851-4b6f0a77d4ef" />

input document 2 

<img width="898" height="441" alt="image" src="https://github.com/user-attachments/assets/95b103c9-3788-4ec7-9d74-b57c99246963" />

output 

<img width="939" height="410" alt="image" src="https://github.com/user-attachments/assets/bb6f7c5f-1adc-43e0-8e0f-21b02b67e504" />
<img width="1025" height="656" alt="image" src="https://github.com/user-attachments/assets/ac0eb5a4-5705-4a62-b593-45de978c21d3" />


input document 3

<img width="885" height="586" alt="image" src="https://github.com/user-attachments/assets/07818b4d-8e71-44cf-a80d-2fbfd1e7f93a" />

output 
<img width="934" height="384" alt="image" src="https://github.com/user-attachments/assets/cfc7e7be-ae7a-498f-a720-1d619081d45f" />
<img width="949" height="542" alt="image" src="https://github.com/user-attachments/assets/be7c2fdf-7909-4d96-88ca-a6067dd38b2d" />


---
---
---


