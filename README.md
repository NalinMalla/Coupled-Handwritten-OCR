An optical character recognition (OCR) software which excels in reading handwritten English text. It <mark>leverages modified versions of various pre-existing OCR technologies like DocTR, PaddleOCR, PyTesseract, and TrOCR which have been stacked to create an optimal pipeline to improve overall performance significantly.</mark> 

To accomplish this, I had to identify the best combination of OCR tools that maximized detection and recognition accuracy, so I started by creating an evaluation module. After this, I had to collect and manually annotate datasets. Additionally, various other support tools like annotation formatter (for converting annotated dataset into usable formats), multi-file OCR, and image processor were also created. Finally, I iteratively trained machine learning models by fine-tuning training parameters to achieve the final product. 

This system was able to <mark>outperform the best available free tools by a remarkable <b>22%</b></mark>. This is illustrated in the following diagram.
![Performance comparison of OCR tools](ocr_performance_comparison.png)
The detailed performance report of these tools can be found in their corresponding <code>eval.json</code> files which are located in the <code>eval_output </code>folder.

Various pre-existing OCR tools were researched for this project. They are listed in the following table.
![Tested OCR tools](Tested_OCR_Tools.png) 

Author: Nalin Malla 
Additional Credit: Thank you Mr. Aayush Baral for training initial version of custom paddle detection model.