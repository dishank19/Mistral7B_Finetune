# Mistral7B_Finetune
Mistral7B finetuned on the SHP dataset

To Replicate Results of the Twitter Polls:
1. Run Preprocess.ipynb and get the reduced_dataset.csv
2. Manual process-  Clean the data, specifically remove text that is not in english, annotate the dataset
3. With the Annotated dataset run TwitterData.ipynb, you might have to clean it again after GPT4 outputs.
Sidenote the create a good instruction prompt, follow this guide: https://lilianweng.github.io/posts/2023-03-15-prompt-engineering/


To replicate Finetuning:

1. For Training: You will need a GPU with atleast 24gb of VRAM, I suggest you rent one using runpod.io
2. Train the model and save relevant checkpoints. The Code for inference is there on the last code block, you can run any query using that. 
3. Test_eval.csv contains the question and its corresponding model and GPT4 output 