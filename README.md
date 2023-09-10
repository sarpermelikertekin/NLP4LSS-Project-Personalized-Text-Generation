# NLP4LSS-Project-Personalized-Text-Generation

The advancement of Large Language Models (LLMs) has started to democratize their use and thus, text generation, widening the fields they are utilized in, ranging from academic writing to business communication. However, one persisting challenge is the lack of style individuality and character in the generated text, which often appears as a blend of various writing styles. Our research aims to overcome this limitation by enabling LLMs to capture and emulate the unique writing style of individuals or entities.,

We explore two main approaches to address this challenge: First, we introduce a novel style embedding layer into the architecture of GPT-2, thereby creating a modified model that theoretically captures the style characteristics of a given entity. Second, we investigate instruction fine-tuning using a more recent LLM, Llama 2, where we explicitly specify the desired style or speaker in the generative instruction.

## Recommended file structure
.
|
-- NLP4LSS Data
   |
   -- hein-daily
|
-- NLP4LSS Script
   |
   -- NLP4LSS-Project-Personalized-Text-Generation
      |
      -- .git
      |
      -- Scripts
         |
         -- Evaluation.ipynb
         |
         -- Finetune_LLama2_7B.ipynb
         |
         -- NLP4LSS Data Processing.ipynb

## DTo Reproduce
- To finetune the model we used a subset of the data provided due to hardware and time constraints.
- To generate this subset one can use the NLP4LSS Data Processing Script
- To get the data first visit the following website https://data.stanford.edu/congress_text and download the hein_daily.zip
- Generate the merged_df for general overviews
- Generate final_df and party_df's
- Feed it to the modell in Finetune_LLama2_7B.ipynb Script
