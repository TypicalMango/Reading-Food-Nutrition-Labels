
# Reading Nutritional Fact Labels on Products
## File Breakdown:
- ###  nutrient-label-ocr.ipynb
Uses EasyOCR along with openCV pre-processing to extract text.<br>
Text is modified to digitally recreate the label.
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
