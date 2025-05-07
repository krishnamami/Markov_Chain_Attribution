# Markov_Chain_Attribution
This project implements a Markov Chain-based attribution model to quantify the impact of each marketing channel on conversions. Unlike traditional attribution models (first-touch, last-touch), this approach dynamically evaluates user journeys and assigns conversion credit based on probabilistic path analysis.

## Business Context
In digital marketing, it’s crucial to understand which touchpoints (ads, channels, or web experiences) truly influence conversions. 

## Example Use case we tried to solve
For QuickenLoans.com, this model can help identify:
- Which A/B test variants or SEO paths drive the most conversions.


![image](https://github.com/user-attachments/assets/9ef05498-a215-425a-bbc9-ed08f651752e)

## Tech Stack:

- **Language**: Python  
- **Libraries**: pandas, numpy, networkx, matplotlib  
- **Model**: Markov Chain (Removal Effect Method)
- **Visualization**: Channel importance and path diagrams

## Understanding Data:

![image](https://github.com/user-attachments/assets/2d47edfb-a04d-46eb-bfe6-19b291a1c145)

## How It Works?:
 * Preprocesses user journeys
   
Below screenshot display sample user journey for each marketing channel
   
   ![image](https://github.com/user-attachments/assets/6a9ca941-8d8c-48f6-8484-9efecbb1ee9a)


* Builds transition states and probabilities
  
Below screenshot displays transition probablities, for example probability of users converting from Instagram is 0.0579

  ![image](https://github.com/user-attachments/assets/c7697055-cf6e-4627-a39d-e86f2e364234)


* Constructs transition matrix

  ![image](https://github.com/user-attachments/assets/33c5c058-7304-4816-9b29-45a721259b99)


* Computes removal effects for each channel

  ![image](https://github.com/user-attachments/assets/c889ac52-8789-4d93-b297-d2ad8de44876)


* Allocates conversion credits proportionally and Visualizes results

  ![image](https://github.com/user-attachments/assets/5b8fb0b4-5922-4c6b-a2aa-9e69271ab7b0)

* Take Aways:

     * This project provided my team with foundational knowledge of Markov Chains and their practical application in marketing attribution.
     * We are currently applying similar principles to a new initiative focused on allocating web experimentation weights to conversions on the QuickenLoans.com website.
     * The goal is to identify which web experiments, in a multi-variant and feature experimentation setup, are positively influencing conversions—and which ones may be negatively impacting user behavior.


How To Run
-->Clone the repo: 

git clone [https://github.com/krishnamami/Markov_Chain_Attribution](https://github.com/krishnamami/Markov_Chain_Attribution.git)

-->pip install -r requirements.txt

-->python markov_attribution_pipeline.py

* Resources
 [Markov Chain Methodology for Attribution – Medium Article](https://medium.com/data-science/marketing-channel-attribution-with-markov-chains-in-python-part-2-the-complete-walkthrough-733c65b23323)


Author: Krishna Goud
 AI & Data Engineering Leader | Head of Data Engineering @ Rocket LA
 
 [LinkedIn](https://www.linkedin.com/in/krishnagoud)
