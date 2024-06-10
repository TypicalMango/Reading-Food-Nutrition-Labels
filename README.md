
# Reading Nutritional Fact Labels on Products
<div style="display: flex; justify-content: space-between;">
  <img src="images/table-1.png" align="top" width="49%" alt="Image 1">
  <img src="images/table-2.png" align="top" width="49%" alt="Image 2">
</div>
<div style="display: flex; justify-content: space-between;">
  <img src="images/table-3.png" align="bottom" width="49%" alt="Image 3">
  <img src="images/table-4.png" align="bottom" width="49%" alt="Image 4">
</div>

## File Breakdown:
- ###  nutrient-label-ocr.ipynb
Uses EasyOCR along with openCV pre-processing to extract text.<br>
Extracted text is modified to digitally recreate the label.
- ### testing-ocr-models.ipynb
Tests the following models:
 - PyTesseract
 - EasyOCR
 - Keras-OCR*
 - docTR*

\* *Didnt work in kaggle environment*

## Known Limitations:
- lack of standardization in label format
- absence of spell checker for extracted output
- OCR fails if label is on highly curved surface
- OCR fails if label isnt bounded by a box
