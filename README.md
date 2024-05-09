# chatgpt-retrieval

Simple script to use ChatGPT on your own files.

## Installation

```
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt 
```

Install [Langchain](https://github.com/hwchase17/langchain) and other required packages.
```
pip install langchain openai chromadb tiktoken unstructured
```
Modify `constants.py` to use your own [OpenAI API key](https://platform.openai.com/account/api-keys). **Important: I recommend a project key with the appropriate rate limits.**

Place your own data into `data/data.txt`.


## Example usage
Test reading `data/data.txt` file.
```
> python chatgpt.py "How can I stake my DOT?"
To stake your DOT tokens, you can access the Stake category in the Staking Dashboard. From there, you can choose to stake as a nominator, join a nomination pool, or do both. Additionally, you can inspect the most recent rewards you have received in the payout section. If you're interested in joining a nomination pool, there is a video tutorial available that walks you through the process, as well as a support article on how to join a pool.
```

Test reading `data/cat.pdf` file.
```
> python chatgpt.py "what is my cat's name"
Your cat's name is Muffy.
```
