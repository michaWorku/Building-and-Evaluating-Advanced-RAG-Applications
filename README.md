# README: Building and Evaluating Advanced RAG Applications  

## 📌 Overview  
This repository contains course notes and notebooks for **Building and Evaluating Advanced RAG Applications**, a deep dive into optimizing **Retrieval Augmented Generation (RAG)** pipelines. The course explores advanced retrieval techniques and evaluation methods to improve **retrieval accuracy, response relevance, and groundedness** in LLM-powered applications.  

## 🛠 What You'll Learn  
- **Advanced Retrieval Methods**  
  - **Sentence-window retrieval**: Enhancing retrieval with surrounding context.  
  - **Auto-merging retrieval**: Structuring hierarchical chunks for better retrieval.  
- **Evaluation and Experimentation**  
  - **RAG Triad**: Measuring **Context Relevance, Groundedness, and Answer Relevance**.  
  - **Iterative evaluation**: Using **TruLens** to refine RAG performance.  
- **Best Practices for RAG Optimization**  
  - Selecting optimal **window sizes** for retrieval.  
  - **Balancing cost and accuracy** in retrieval pipelines.  
  - **Mitigating hallucinations** in LLM-generated responses.  


## 🏗 Course Content  

### [**1️⃣ Advanced RAG Pipeline**](https://github.com/michaWorku/Building-and-Evaluating-Advanced-RAG-Applications/blob/main/L1-Advanced_RAG_Pipeline.ipynb)  
- **Basic RAG Setup**: Using **LlamaIndex** for standard retrieval.  
- **Evaluation Benchmarking**: Setting up **TruEra & TruLens** for evaluation.  
- **Advanced Retrieval Techniques**:  
  - **Sentence-window retrieval**: Incorporating nearby text for better retrieval.  
  - **Auto-merging retrieval**: Merging fragmented chunks into hierarchical structures.  

### [**2️⃣ RAG Evaluation: The RAG Triad**](https://github.com/michaWorku/Building-and-Evaluating-Advanced-RAG-Applications/blob/main/L2-RAG_Triad_of_metrics.ipynb)  
The **RAG Triad** evaluates LLM-generated responses based on:  
- **Answer Relevance**: Is the response relevant to the query?  
- **Context Relevance**: Is the retrieved context accurate?  
- **Groundedness**: Is the response properly supported by retrieved context?  

#### **Evaluation Process**  
1. Start with a **basic RAG pipeline** (LlamaIndex).  
2. **Evaluate with TruLens** using the RAG Triad.  
3. Identify **failure modes** (e.g., issues due to context size).  
4. **Iterate with advanced retrieval** (Sentence-window, Auto-merging).  
5. **Re-evaluate and compare metrics** to measure improvements.  
6. **Experiment** with different retrieval settings (e.g., window size, chunk structure).  

### [**3️⃣ Sentence-Window Retrieval**](https://github.com/michaWorku/Building-and-Evaluating-Advanced-RAG-Applications/blob/main/L3-Sentence_window_retrieval.ipynb)  
- Improves **retrieval accuracy** by incorporating **context from surrounding sentences**.  
- Uses **sentence windows** to balance **token cost vs. information depth**.  
- Evaluation:  
  - Test with **different window sizes** (1, 3, 5).  
  - Assess impact on **Context Relevance & Groundedness**.  

### [**4️⃣ Auto-Merging Retrieval**](https://github.com/michaWorku/Building-and-Evaluating-Advanced-RAG-Applications/blob/main/L4-Auto-merging_Retrieval.ipynb)  
- Structures retrieval with a **hierarchical chunking approach**.  
- Merges **smaller chunks** when a threshold is reached, improving coherence.  
- Evaluation:  
  - Experiment with **different chunking hierarchies**.  
  - Measure improvements in **retrieval efficiency & answer quality**.  


## 🔬 Experimentation & Evaluation  
- **TruLens** for tracking RAG pipeline performance.  
- **Key Metrics Evaluated**:  
  - **Honesty**: Answer Relevance, Embedding Distance, Summarization Quality, BLUE, ROUGE,Context relevance, Groundedness, Custom evaluation.  
  - **Harmlessness**: PII Detection, Toxicity, Jailbreaks, Custom evaluations.  
  - **Helpfulness**: Sentiment, Language mismatch,Coherence, Conciseness, Custom evaluations.  


## 🚀 Getting Started  
1. **Clone the repository**  
   ```bash
   git clone https://github.com/michaWorku/Building-and-Evaluating-Advanced-RAG-Applications.git
   cd your-repo-folder
   ```
2. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the Jupyter Notebook**  
   ```bash
   jupyter notebook
   ```


## 📚 References  
- [LlamaIndex Documentation](https://docs.llamaindex.ai/en/stable/)  
- [TruLens Evaluation Framework](https://www.trulens.org/getting_started/) 
- [DeepLearning.AI Course](https://www.deeplearning.ai/short-courses/building-evaluating-advanced-rag/)  


## 💡 Conclusion  
This course provides a **practical and systematic approach** to building **robust, high-performing RAG applications**. By implementing **advanced retrieval techniques** and **evaluation frameworks**, you can **enhance accuracy, reduce hallucinations, and optimize response quality** in LLM applications. 🚀  
