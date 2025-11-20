# Normalization Techniques in Python  
### Comparing Max Scaling, Min-Max Scaling, and Standardization

This project demonstrates three widely used normalization techniques applied to a small dataset using Python and Pandas. Normalization is a key preprocessing step in data science and machine learning, especially when features have very different scales.

The dataset used here contains four columns with values on very different ranges. This makes it an ideal example to illustrate why normalization is necessary and how different techniques affect feature scaling.

---

## Overview

Machine learning algorithms often assume that all features contribute equally, but this is not the case when variables have very different magnitudes. To address this, normalization transforms data into standardized ranges.

In this notebook, we compare three techniques:

- **Max Scaling**  
- **Min-Max Scaling**  
- **Standardization (Z-score normalization)**  

Each technique affects the data differently and is suitable for different types of models.

---

## What the Notebook Covers

### 1. Create a Sample Dataset

A Pandas DataFrame is constructed with four columns of numerical values:

```python
df = pd.DataFrame([
    [180000, 110, 18.9, 1400], 
    [360000, 905, 23.4, 1800], 
    [230000, 230, 14.0, 1300], 
    [60000,  450, 13.5, 1500]
], columns=['Col A', 'Col B', 'Col C', 'Col D'])
