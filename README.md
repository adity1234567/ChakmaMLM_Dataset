# Bangla-transliterated Chakma Corpus

## Overview
This dataset contains a **Bangla-transliterated Chakma corpus** curated from Chakma books and manually validated.  
We used the dataset in the paper:  
*Exploring Cross-Lingual Knowledge Transfer via Transliteration-Based MLM Fine-Tuning for Critically Low-resource Chakma Language*.

The dataset is designed for **low-resource language adaptation research**.  

---

## Dataset Description

- **Language:** Chakma language written in **Bangla script (transliteration)**  
- **Sources:** 4 Chakma books 
- **Collection Methods:**  
  - PyTesseract OCR  
  - Gemini 2.5 Pro OCR  
  - Manual curation and correction  
- **Manual Validation:** 4,570 sentences validated by native speakers  

---


| Dataset Version      | Total Sentences | Notes |
|----------------------|-----------------|-------|
| **Tesseract OCR**    | 6,353           | Raw OCR output |
| **Gemini OCR**       | 5,982           | Raw OCR output |
| **Manually Corrected** | 4,570           | Manually cleaned dataset |

**Book-wise Breakdown (Manually Corrected):**
- Book 3 (Full): 3,287 sentences  
- Book 2 (Partial): 1,283 sentences  

---

## Sources of The Books

<img width="1226" height="405" alt="image" src="https://github.com/user-attachments/assets/e2b66161-6d1b-4632-a0b0-472375e4cb66" />


## Data Format

- Files are in **plain text (.txt)**  
File Structure:  

```
data/
├── tesseract/
│ ├── book1.txt
│ ├── book2.txt
│ ├── book3.txt
│ └── book4.txt
├── gemini/
│ ├── book1.txt
│ ├── book2.txt
│ ├── book3.txt
│ ├── book4.txt
└── manual/
├── book2_partial.txt
├── book3_full.txt

---

## Train/Eval/Test Split

| Dataset  | Train | Eval | Test |
|----------|-------|------|------|
| Tesseract OCR | 4,348 | 832  | 1,173 |
| Gemini OCR    | 3,815 | 994  | 1,173 |
| Manual Fixed  | 2,908 | 545  | 1,118 |

---
```
<!--## Applications

- Pretraining & fine-tuning multilingual LMs for Chakma   
- Tokenization and morphology analysis in Indic scripts  
- Evaluation of OCR quality in low-resource settings  

---
-->
## License
The dataset is released for **research purposes only**. Please cite our paper when using it.  

---

## Citation
If you use this dataset, please cite:

@article{khisa2025exploring,
  title={Exploring Cross-Lingual Knowledge Transfer via Transliteration-Based MLM Fine-Tuning for Critically Low-resource Chakma Language},
  author={Khisa, Adity and Jahan Lia, Nusrat and Mahfuz Nafis, Tasnim and Masud, Zarif and Pial, Tanzir and Rayana, Shebuti and Kabir, Ahmedul},
  journal={arXiv e-prints},
  pages={arXiv--2510},
  year={2025}
}


```
