# NewsInsight

NewsInsight is a powerful and efficient news research tool that leverages the capabilities of Streamlit, LangChain, OpenAI embeddings, and FAISS to provide accurate and swift answers to your queries based on recent news articles. This tool is designed to help you stay updated with the latest news and extract relevant information effortlessly.

## Features

- **Load URLs** or upload text files containing URLs to fetch article content.
- **Process Article Content** through LangChain's UnstructuredURLLoader.
- **Generate Embedding Vectors** using OpenAI's embeddings.
- **Efficient Retrieval** of relevant information using FAISS, a powerful similarity search library.
- **Interact with LLM (ChatGPT)** by inputting queries and receiving answers along with source URLs.

## Usage

1. **Run the Streamlit app** by executing:
   ```bash
   streamlit run main.py
   ```
2. **Open the web app** in your browser.
3. **Input URLs** directly on the sidebar.
4. **Process URLs** by clicking the "Process URLs" button.
5. **Observe the system** as it performs text splitting, generates embedding vectors, and indexes them using FAISS.
6. **Ask a question** and get the answer based on those news articles.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/NewsInsight.git
   cd NewsInsight
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Streamlit app:
   ```bash
   streamlit run main.py
   ```

## How It Works

1. **Load Articles**: Load URLs or text files containing URLs to fetch news articles.
2. **Text Splitting**: Articles are split into manageable chunks.
3. **Embedding Vectors**: Generate embedding vectors using OpenAI's embeddings.
4. **Indexing with FAISS**: Efficiently index the embedding vectors using FAISS.
5. **Question Answering**: Input queries and receive answers based on the indexed news articles.

## Example

### Input URLs
- [Tata Motors and Mahindra Gain Certificates for Production-Linked Payouts](https://www.moneycontrol.com/news/business/tata-motors-mahindra-gain-certificates-for-production-linked-payouts-11281691.html)
- [Tata Motors Launches Punch ICNG](https://www.moneycontrol.com/news/business/tata-motors-launches-punch-icng-price-starts-at-rs-7-1-lakh-11098751.html)
- [Buy Tata Motors, Target of Rs 743 - KR Choksey](https://www.moneycontrol.com/news/business/stocks/buy-tata-motors-target-of-rs-743-kr-choksey-11080811.html)

### Question
- Summarize KR Choksey's report on Tata Motors.

### Answer
- KR Choksey's report on Tata Motors states that the company is expected to grow at a CAGR of 17.5%/40.1% in revenues/EBITDA over FY23-25E. The report values the JLR & Chery-JLR JV businesses at 2.4x EV/EBITDA, TML-CV at 13.0x EV/EBITDA, and TML-PV business at 14.5x EV/EBITDA, and a value of INR 40 per share for stake in Tata Technologies. The report estimates a target price of INR 743 per share with an upside of 15.4% and gives a “BUY” rating on the shares of Tata Motors.

## Contributing

We welcome contributions from the community. If you have any suggestions, bug reports, or feature requests, please open an issue or submit a pull request.
