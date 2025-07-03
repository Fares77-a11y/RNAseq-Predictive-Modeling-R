# RNAseq-Predictive-Modeling-R
Classification analysis of RNA-seq data using custom caret SBF pipelines with C5.0 and Random Forest models, evaluated by LOOCV.
# 🧠 RNA-seq Classification Analysis using C5.0 and Random Forest in R

This project demonstrates how to apply supervised machine learning algorithms to RNA-seq data, including **decision trees (C5.0)** and **random forests**, using custom feature selection and leave-one-out cross-validation (LOOCV). The workflow is fully scripted in base R and `caret` without `miodin`, and features a modular classification strategy with performance benchmarking against baseline guessing.

---

## 📌 Project Highlights

- Custom feature selection via Coefficient of Variation (CoV)
- Search-By-Filter (SBF) control setup using `caret`
- Model training with C5.0 and Random Forest
- Evaluation using confusion matrices, sensitivity, specificity, and Kappa
- Assessment against random guessing baseline

---

## 🧠 Skills Demonstrated

- Feature engineering and filter-based selection
- ML modeling using `caret::sbf()` with LOOCV
- Critical comparison of classifier performance
- Pipeline reproducibility in base R

---

## 📈 Performance Comparison

Below is a comparison of the two classification models built on high-dimensional RNA-seq data:

| Model              |   Accuracy |   Sensitivity |   Specificity |   Kappa | Better than Blind Guessing   |
|:-------------------|-----------:|--------------:|--------------:|--------:|:-----------------------------|
| C5.0 Decision Tree |       0.8  |          0.75 |          0.83 |    0.6  | Yes                          |
| Random Forest      |       0.93 |          0.9  |          0.95 |    0.86 | Yes                          |

📄 Also available as: [`model_performance_comparison.csv`](results/model_performance_comparison.csv)

---

## 📂 Project Structure

```
RNAseq-Classification-Models/
├── src/
│   └── RNAseq_Classification_Analysis.Rmd
├── results/
│   └── model_performance_comparison.csv
├── data/
│   └── a23farib_rnaseq.txt

```

---

## 🚀 How to Run

1. Open the `.Rmd` file in RStudio  
2. Install required packages:
```r
install.packages("caret")
install.packages("C50")
```
3. Run all code chunks or knit to HTML

---

## 👨‍💻 Author

**Fares Ibrahim**  
Bioinformatician | ML in Biology | Cancer Transcriptomics  
🔗 [GitHub](https://github.com/Fares77-a11y)

---

## 📄 License

MIT License — see `LICENSE` file for terms.
