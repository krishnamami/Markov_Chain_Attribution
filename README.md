# Markov_Chain_Attribution
A Python implementation of the Markov Chain Attribution Model for analyzing marketing channel effectiveness using customer journey data. This project helps quantify how each channel contributes to conversions by simulating the impact of removing them from the conversion path.

# What is Markov?
Unlike simple rule-based models such as first-touch or last-touch attribution, the Markov Attribution Model takes a probabilistic approach by analyzing entire user journeys.

It calculates the removal effect — the decrease in the overall conversion rate when a specific channel is removed from the path. This allows you to quantify each channel’s true influence on conversions by understanding how essential it is to the customer journey.

In short : "What happens to conversion performance if this channel didn’t exist?”

![image](https://github.com/user-attachments/assets/9ef05498-a215-425a-bbc9-ed08f651752e)

# Understanding Data:

![image](https://github.com/user-attachments/assets/2d47edfb-a04d-46eb-bfe6-19b291a1c145)

# How It Works?:
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
