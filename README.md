## Sentiment Analysis using BERT Hugging Face

### Software And Tools Requirements

1. [Github Accouunt](https://github.com)
2. [VS Code IDE](https://code.visualstudio.com)
3. [Git CLI](https://git-scm.com/book/en/v2/Getting-Started-The-Command-Line)
4. [Hugging Face](https://huggingface.co/)
5. [Pytorch](https://pytorch.org/get-started/locally/)

Create a new environment

```
conda create -p venv python==3.7 -y
```

Install Pytorch version 

```
conda install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia
```

Steps 

```
1. Install required dependencies as mentioned above
2. Initiate the model from Hugging Face - (https://huggingface.co/nlptown/bert-base-multilingual-uncased-sentiment)
3. Select the web page to analyze sentiment of the reviews
4. Use Beautifulsoup Python package for parsing HTML page
5. Collect the reviews using Regex
6. Load reviews into DataFrame
7. Tokenize the reviews to get tokens and pass those tokens through model to get result
8. Find the maximum value from logits of result (result.logits)
9. The sentiment score varies between 1 to 5 (1-most Negative, 3-Neutral, 5-most Positive)
7. Showcase the reviews and its sentiments in the dataframe
```
