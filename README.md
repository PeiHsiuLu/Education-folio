# Education Big Data Project Production  
### Department: 115 Technology and Human Resources 
### Name: Pei-Hsiu Lu (呂沛修)  
### Instructor: Professor Yun-Chen Tsai (蔡芸琤教授)  

## 6/27 (Third Class)
### Practice 1: Retrieving Models from Huggingfacehub

**Model retrieved:** stable-diffusion-v1-5 (text to image)  
**Model test and modifications:** [Notebook link](https://github.com/PeiHsiuLu/Education-folio/blob/main/big_data.ipynb)

**Modifications made:** 
The original model generated a single image from text input. I attempted to make it more interactive by allowing users to input text and generate specific images.

**Additional resources:** 
LangChain, Tavily AI

## 6/27 (Fourth Class)
### Practice 2: Gimini AI

**Supplementary resources:**  
1. Gimini AI  
2. Gradio  

You can find related videos online to learn by yourself (search for content similar to your project).

## Self-study on 7/2

### Hugging Face (image to image)  
**Post-class attempt:** [Hugging Face Notebook](https://github.com/PeiHsiuLu/Education-folio/blob/main/Hugging_face_image2image.ipynb)  
**Model used:** stabilityai/stable-diffusion-xl-refiner-1.0

## Self-study on 7/3

### LangChain
1. Aiming to provide developers with tools and interfaces to more easily and effectively utilize large language models (LLM) within an open-source framework.
2. Mainly includes libraries for JS and Python.
3. In short, it provides an interface for users to easily use AI models directly without spending additional time on training.

LangChain aims to provide developers with tools and interfaces to more easily and effectively utilize large language models (LLM) within an open-source framework. It mainly includes libraries for JavaScript and Python, allowing developers to use LLMs easily within these common programming languages. In short, LangChain offers an interface that makes it easier for users to use pre-trained AI models directly, without needing to spend additional time on training. Additionally, LangChain provides various tools and examples to help developers quickly build and deploy applications.

## Project Production on 7/4
### Applying Hugging Face Model: openai/whisper-large-v3 (speech to text)
First, I downloaded the videos and converted them to mp3 audio files, then converted the audio to text output.  
**Voice to Text:** [Notebook link](https://github.com/PeiHsiuLu/Education-folio/blob/main/Educationfolio_project.ipynb)

## Project Production

### Topic: Feedback Generator
**Description:**
Allows users to upload audio files or text, and the AI can generate reasonable feedback based on the uploaded content.

**Motivation/Purpose:**
To address students' needs for writing feedback assignments and to learn English (my personal need).

**Other features:**
1. Set the required number of words.
2. Set the sentiment of the content.
3. Set the stance level (positive/negative).
4. Option to include scores (generated based on stance data).
5. Use feedback to learn English.

### Startup Method
1. Click the "Code" button and select "Download ZIP".
2. Unzip the downloaded file.
3. Run aiproject_v4.(gemini-1.5-pro).py (requires ffmpeg and relevant package imports).
4. Watch the introduction video for usage instructions.

### Additional Notes
In version 4, there may be overfitting in the "feeling" part. Using the paid version of Gemini can resolve this by training with the entire CSV dataset.  
[Main results of the project](https://github.com/SAStommy/eduAIproject/tree/main)

### Division of Work
**Pei-Hsiu Lu's responsibilities:** Data collection, organizing positive and negative sentiment labels (500 entries for training, 500 for validation), fine-tuning the model based on generated results and making manual adjustments.  
**Ming-Feng Tu's responsibilities:** Coding, Gradio frontend, fine-tuned model.

### Reflection
**Reflection on the project:**  
I found that the most exhausting part of data collection was the sheer volume of data needed. Additionally, considering the need for diverse data and sentiment in feedback was challenging. Moreover, web scraping might gather too many repetitive course reviews, which might not be beneficial for AI model training. Therefore, manual data collection was necessary in the end.

**Validation data:** [Validation Data](https://github.com/PeiHsiuLu/Education-folio/blob/main/0714_education.csv)  
**Training data:** [Training Data](https://github.com/PeiHsiuLu/Education-folio/blob/main/0714_train.csv)  

**Reason for using only 100 out of 500 entries:** Due to token limitations in Gemini, only a small amount of data could be used for training.  
**Reason for not using validation data:** The dataset was too small, with only 100 entries for training, making validation impractical.  
We did not use validation data because the dataset was too small, with only 100 entries for training, making effective validation impossible.

### Final Project Presentation Video
[Feedback Generator](https://www.youtube.com/watch?v=ZhsbQv5_M1o)

