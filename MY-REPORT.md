![GenI-banner](https://github.com/genilab-fau/genilab-fau.github.io/blob/8d6ab41403b853a273983e4c06a7e52229f43df5/images/genilab-banner.png?raw=true)

# **Research Report: Multi-Level Prompt Engineering for Chatbot Requirement Analysis**

* Authors: Anudeep Reddy Raavi, Akhila Manthena, Suresh Puchagatla.
* Academic Supervisor: [Dr. Fernando Koch](http://www.fernandokoch.me)

# Research Question

Can **Automatic Prompt Engineering (APE)** and **ReAct (Reasoning + Acting)** improve chatbot requirement analysis, and which performs best under varying model configurations?

## Arguments

#### What is already known about this topic

* Prompt Engineering significantly impacts  AI-generated responses .
* Automatic Prompt Engineering (APE) allows AI to  generate its own prompts , removing human bias.
* ReAct (Reasoning + Acting) iteratively breaks down problems before generating responses, leading to  better-structured outputs .
* Different model parameters (temperature, context, max predictions) can alter response  coherence, creativity, and precision .

#### What this research is exploring

* We employ APE and ReAct to  generate chatbot requirement analysis .
* We compare their performance using  execution time, response length, and content quality .
* We test variations in temperature, context size, and prediction length to analyze effectiveness.

#### Implications for practice

* It will optimize the process of requirement analysis generation for chatbot projects.
* It will provide insights into which  prompting technique is best suited for structured AI-generated reports .
* It enables automation in prompt optimization, reducing the need for manual intervention.

# Research Method

* **Multi-Level Prompt Engineering Setup**
  * **Step 1**: Generate  structured prompts using APE .
  * **Step 2**: Generate  iterative responses using ReAct .
  * **Step 3**: Execute  both techniques with different model configurations .
* **Parameter Variations**
  * **Temperature**: 0.7 (more deterministic) vs. 1.2 (more creative).
  * **Context Size**: 500 vs. 600 tokens.
  * **Max Predictions**: 700 vs. 800 tokens.
* **Evaluation Metrics**
  * Execution Time (speed of response generation).
  * Response Length (detailed vs. concise outputs).
  * Coherence & Completeness (subjective evaluation).

# Results

Describe the results achieved through your research process.

| **Technique** | **Configuration**               | **Execution<br /> Time** | **Response<br />Length** | **Observations**      |
| ------------------- | ------------------------------------- | ------------------------------ | ------------------------------ | --------------------------- |
| APE                 | Temp: 0.7, Context: 500, Predict: 700 | 15.83s                         | 3677 characters                | Structured and clear        |
| APE                 | Temp: 1.2, Context: 600, Predict: 800 | 15.02s                         | 3551 characters               | More creative but verbose   |
| ReAct               | Temp: 0.7, Context: 500, Predict: 700 | 12.29s                         | 2419 characters               | More detailed, step-by-step |
| ReAct               | Temp: 1.2, Context: 600, Predict: 800 | 12.26s                         | 2222 characters                | Iterative and in-depth      |

# Further research

* Testing different AI models (GPT-4, Gemini, Mixtral) for cross-model comparisons.
* Implementing a scoring algorithm for coherence, accuracy, and completeness.
