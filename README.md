## Intelligent Frequently Asked Questions Software


### Project Description
Swinburne Online is a digital education portal that delivers online university and TAFE courses on behalf of Melbourne’s Swinburne University of Technology
(RTO 3059), one of Australia’s leading educational institutions with over 30,000 students. The website of Swinburne Online handles tens of thousands of visits for
general enquires. There is a traditional Frequently Asked Questions (FAQ) website on Swinburne Online, which is a collection of commonly asked questions
and answers. Users usually need to browse through many questions before they can find the answer they are looking for, whilst questions and answers are
organized by topic. This may cause a certain impact on user experience and satisfaction, and ultimately affected users’ interests. In this project, we would like
to provide an intelligent workflow for Swinburne Online FAQ website to communicate clearly and effectively, and to provide friendly and professional customer service.


## Motivation
There is a Swinburne Online FAQs website where student can flip through all kinds of frequently asked questions along with corresponding answers to get accurate information they need. 
But every time they have a question, the student has to find out similar question by checking questions from beginning of website to the end, which is a time-consuming process and frustrating experience to every student. 
To address the pain point of Swinburne Online student who frequently asked questions, an intelligent question and answering workflow is needed to help students get answers to questions quickly and efficiently.


### Technology used
#### Model
-BERT
-LLAMA2-7b-chat-hf

#### Data Preprocessing
-Data augmentation
-Data annotation
-Data conversion
-SQUAD

#### Model Fine-tuning
Fine-tune Llama2-7b-chat-hf model on a T4 GPU with high RAM using Google Colab (Pro). Due to high consumption of VRAM from Llama2 model, parameter-efficient fine-tuning (PEFT) techniques like LoRA or QLoRA were needed. 
To significantly lower VRAM usage, fine-tuning the model in 4-bit precision is necessary, and that is where QLoRA comes into play. 
The advantage is that I can make use of the Hugging Face ecosystem, including the transformers, accelerate, peft, trl, and bitsandbytes libraries.

