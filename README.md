
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
- different formatting of labels
- doesnt spell check extracted output
- if label is on highly curved surface, OCR fails (image 1 of dataset)
- if label isnt bounded by a box, OCR fails (image 2 of dataset)
