[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/bn-drishti-bangla-document-recognition/handwritten-line-segmentation-on-bn-htrd)](https://paperswithcode.com/sota/handwritten-line-segmentation-on-bn-htrd?p=bn-drishti-bangla-document-recognition)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/bn-drishti-bangla-document-recognition/handwritten-word-segmentation-on-bn-htrd)](https://paperswithcode.com/sota/handwritten-word-segmentation-on-bn-htrd?p=bn-drishti-bangla-document-recognition)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/bn-drishti-bangla-document-recognition/handwritten-word-segmentation-on)](https://paperswithcode.com/sota/handwritten-word-segmentation-on?p=bn-drishti-bangla-document-recognition)
[![Generic badge](https://img.shields.io/badge/State_of_the_Art-On_ICDAR_2013_Handwriting_Segmentation_Dataset-<COLOR>.svg)](https://users.iit.demokritos.gr/~nstam/ICDAR2013HandSegmCont/resources.html)
[![Generic badge](https://img.shields.io/badge/State_of_the_Art-Handwritten_Word_and_Line_Segmentation_on_WBSUBNdb\_text-<COLOR>.svg)](https://github.com/Chayan-halder/WBSUBNdb_text---Bangla-handwritten-text-document-dataset)

# **BN-DRISHTI**
**BN-DRISHTI:** **B**a**n**gla **D**ocument **R**ecognition through **I**nstance-level **S**egmentation of **H**andwritten **T**ext **I**mages

## How To Run The **DEMO** (Inferencing on Single Image):
1) Open the [**BN_DRISHTI_DEMO.ipynb**](https://github.com/crusnic-corp/BN-DRISHTI/blob/main/BN_DRISHTI_DEMO.ipynb) script and click on the **Open In Colab** Button.
2) Run the script from **Runtime ->  Run All**
3) Download some Handwritings from the **sample_image** of the repository. Or supply your own. 
4) UPLOAD ONE Image (per-run) containing Handwritings (from your device) by clicking on **Choose Files** button once the cells are executing.
	
You can see different transitions/outputs by going through the cells.

## Running Bulk Inferencing (on unannotated images):
1) Open the [**BN_DRISHTI_Bulk_Inferencing.ipynb**](https://github.com/crusnic-corp/BN-DRISHTI/blob/main/bulk_inferencing/BN_DRISHTI_Bulk_Inferencing.ipynb) script from 'bulk_inferencing' folder and click on the **Open In Colab** Button.
2) Run the script from **Runtime ->  Run All**
3) By default it is executed on the **bulk_sample.zip** data but you can supply your own .zip file through a link. 
4) The outputs will be saved on the temporary space in CoLab.
5) You can also save the output on your google drive or download them as .zip by uncommenting either of the last two cells.

## Reproducing Results on BN-HTRd **Test Dataset** (with ground truths):
1) Open the [**BN_DRISHTI_Run_On_Test_Sets.ipynb**](https://github.com/crusnic-corp/BN-DRISHTI/blob/main/test_scripts/BN_DRISHTI_Run_On_Test_Sets.ipynb) script from 'test_scripts' folder and click on the **Open In Colab** Button.
2) Run the script from **Runtime ->  Run All**
3) By default it is executed on the **test.zip** data but you can supply your own .zip file through a link.
4) If you use your own dataset you also have to supply ground truths (please follow folder structure like test.zip).
5) The outputs will be saved on the temporary space in CoLab.
6) You can also save the output on your google drive or download them as .zip by uncommenting either of the last two cells.

## MODEL Files:
- The custom [YOLOv5](https://github.com/ultralytics/yolov5/wiki/Train-Custom-Data) models trained on the BN-HTRd Dataset for **line and word segmentation** will be automatically downloaded when you run the script.
- If you want to download the Trained Models you can visit our Hugging Face Model Hub:
	- [BN-DRISHTI Line/Word Segmentation Models](https://huggingface.co/crusnic/BN-DRISHTI/tree/main/models)
- [**Try Out Live Demo for YOLO Models Only**](https://bn-htr-yolo.streamlit.app/):
	- By **Default** the selected model will be *Downloaded Automatically* from our [HuggingFace Model Hub](https://huggingface.co/crusnic/BN-DRISHTI/tree/main/models).
	- You can also use your own model (.pt) file through **File Upload** option while running the demo.
 	<br>**OR**</br>
	- You can paste the models **Link** directly to the **URL** option, for example:
  		- Line Model: `https://huggingface.co/crusnic/BN-DRISHTI/resolve/main/models/line_model_best.pt`
  		- Word Model: `https://huggingface.co/crusnic/BN-DRISHTI/resolve/main/models/word_model_best.pt`
	
**Note:** You will not be able to get perfect results by only using the YOLO models.
- Please check our scripts and methods for more details [**BN-DRISHTI PAPER**](https://arxiv.org/abs/2306.09351).

## Dataset:
- We primarily used the [BN-HTRd](https://data.mendeley.com/datasets/743k6dm543) Dataset (v4.0) - for Training/Evaluating our models.
- You can find the exact Splitted Dataset in our Hugging Face Dataset Hub:
	- [BN-HTRd_Splitted Dataset for Model Building](https://huggingface.co/datasets/shaoncsecu/BN-HTRd_Splitted)
	
	
 ## To Cite the Dataset Paper:
 ```ruby
@incollection{rahman2023bn,
      title={BN-HTRd: A Benchmark Dataset for Document Level Offline Bangla Handwritten Text Recognition (HTR) and Line Segmentation},
      author={Rahman, Md Ataur and Tabassum, Nazifa and Paul, Mitu and Pal, Riya and Islam, Mohammad Khairul},
      booktitle={Computer Vision and Image Analysis for Industry 4.0},
      pages={1--16},
      year={2023},
      publisher={CRC Press 6000 Broken Sound Parkway NW, Suite 300, Boca Raton, FL 33487-2742}
}
```

 ## To Cite the **BN-DRISHTI** Paper:
 ```ruby
@InProceedings{10.1007/978-3-031-41501-2_14,
      author="Jubaer, Sheikh Mohammad and Tabassum, Nazifa and Rahman, Md Ataur and Islam, Mohammad Khairul",
      editor="Coustaty, Mickael and Forn{\'e}s, Alicia",
      title="BN-DRISHTI: Bangla Document Recognition Through Instance-Level Segmentation of Handwritten Text Images",
      booktitle="Document Analysis and Recognition -- ICDAR 2023 Workshops",
      year="2023",
      publisher="Springer Nature Switzerland",
      address="Cham",
      pages="195--212"
}
```

