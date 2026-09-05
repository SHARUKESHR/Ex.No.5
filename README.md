# EXPERIMENT 5: Comparing Prompting Techniques Through Engineering Problem-Solving Scenarios

## Aim

To compare different prompting techniques and evaluate their effectiveness in solving a real-world engineering problem selected from a 3rd-year/final-year engineering project by analysing the quality, accuracy, depth, clarity, feasibility, and usefulness of AI-generated responses.


## Project Title

### GENERATIVE AI FOR DEMYSTIFYING LEGAL DOCUMETS

## Selected Engineering Scenario

### Problem Statement

Legal documents such as rental agreements, employment contracts, terms and conditions, and legal notices often contain complex legal terminology and lengthy sentences that are difficult for ordinary users to understand. The project aims to use Generative AI to simplify legal language, identify important clauses, explain their meaning in simple terms, and highlight potential risks or obligations.

For the prompting experiment, the same legal document or legal clause can be given to an AI system using different prompting techniques, and the resulting responses can be compared.




## Requirement Analysis

For the project “Generative AI for Demystifying Legal Documents,” requirement analysis identifies the hardware, software, functional, and non-functional requirements needed to develop a system that can process complex legal documents and explain them in simple language.

### 1. Functional Requirements
   
Document Upload – The system should allow users to upload legal documents such as PDF, DOCX, or text files.
Document Text Extraction – The system should extract readable text from the uploaded legal document.
Legal Document Analysis – The system should analyze the extracted content and identify important clauses, terms, obligations, and conditions.
Simplification – The Generative AI model should convert complex legal language into simple and understandable language.
Clause Explanation – The system should provide explanations for individual legal clauses when requested by the user.
Key Information Identification – The system should highlight important information such as dates, penalties, responsibilities, rights, fees, and termination conditions.
Question Answering – Users should be able to ask questions about the uploaded document and receive answers based on its contents.
Risk/Concern Identification – The system can identify potentially important or concerning clauses and explain why they may require attention.
Summary Generation – The system should generate a concise summary of the entire document.
User-Friendly Output – Results should be presented in a clear format using headings, bullet points, and simple language.

### 2. Non-Functional Requirements

Accuracy: The generated explanation should remain faithful to the original legal document.
Clarity: The output should be understandable to users without legal knowledge.
Performance: The system should process documents and generate responses within a reasonable time.
Security: Uploaded legal documents and user information should be protected from unauthorized access.
Scalability: The system should be capable of handling documents of different sizes and types.
Usability: The interface should be simple and easy to navigate.
Reliability: The system should provide consistent results for similar inputs.
Privacy: User-uploaded legal documents should not be unnecessarily exposed or shared.

### 3. Hardware Requirements

Processor: Intel Core i5 or equivalent
RAM: Minimum 8 GB
Storage: Minimum 256 GB
Internet: Required for accessing Generative AI/API services
Display: Standard monitor or laptop display

### 4. Software Requirements

Operating System: Windows/Linux/macOS
Programming Language: Python
Frontend: HTML, CSS, JavaScript / Streamlit
Backend: Python-based application
AI Model: Generative AI/LLM
Document Processing: PDF/DOCX text extraction libraries
Database: SQLite/MySQL or another suitable database, if required
Development Environment: VS Code/Jupyter Notebook
API: Generative AI API for document analysis and response generation

### 5. User Requirements

The user should be able to:

Upload Document → Extract Text → Analyze Legal Content → Simplify Clauses → View Summary → Ask Questions → Receive Explanations

The system should also clearly indicate that its output is intended for understanding and informational purposes and is not a substitute for advice from a qualified lawyer.# RESULT

## Architecture Flow

User → Document Upload → Text Extraction → Preprocessing → Prompt Engineering → Generative AI Model → Legal Analysis → Simplification & Summary → User Interface

### 1. User Interface Layer

The user interacts with the system through a web-based interface. The user can upload a legal document and request operations such as summarization, clause explanation, key-point extraction, and question answering.

### 2. Document Processing Layer

The uploaded document is processed to extract its textual content. PDF, DOCX, or text documents can be converted into machine-readable text. Unnecessary spaces, symbols, and formatting issues can then be removed during preprocessing.

### 3. Prompt Engineering Layer

The extracted legal content is combined with carefully designed prompts. Different prompting techniques such as zero-shot, few-shot, role-based, and constraint-based prompting can be applied to determine how each technique affects the quality of the generated response.

### 4. Generative AI Layer

The processed text and prompt are provided to a Large Language Model (LLM). The model analyzes the document and generates a response based on the user's request.

### 5. Legal Information Analysis Layer

The generated output focuses on useful information such as:

Important clauses
Rights and responsibilities
Obligations
Payment terms
Penalties
Deadlines
Termination conditions
Potential areas requiring attention
### 6. Output Generation Layer

The complex legal information is converted into simple, user-friendly explanations. The system can provide a document summary, clause-by-clause explanation, or answers to user questions.

### 7. Evaluation Layer

For the prompting experiment, outputs generated using different prompting techniques are compared using:

Relevance → Accuracy → Completeness → Clarity → Feasibility → Usefulness

The best-performing prompting technique can then be identified for the proposed system.

#### Simple Architecture Diagram

             ┌──────────────────┐
             │      USER        │
             └────────┬─────────┘
                      │
                      ▼
             ┌──────────────────┐
             │ Document Upload  │
             └────────┬─────────┘
                      │
                      ▼
             ┌──────────────────┐
             │ Text Extraction  │
             └────────┬─────────┘
                      │
                      ▼
             ┌──────────────────┐
             │ Preprocessing    │
             └────────┬─────────┘
                      │
                      ▼
             ┌──────────────────┐
             │ Prompt Engineering│
             │ Zero/Few/Role etc.│
             └────────┬─────────┘
                      │
                      ▼
             ┌──────────────────┐
             │ Generative AI /  │
             │      LLM         │
             └────────┬─────────┘
                      │
                      ▼
             ┌──────────────────┐
             │ Legal Analysis   │
             └────────┬─────────┘
                      │
          ┌───────────┼───────────┐
          ▼           ▼           ▼
      Summary     Explanation   Q&A
          │           │           │
          └───────────┼───────────┘
                      ▼
             ┌──────────────────┐
             │ Simple & Clear   │
             │     Output       │
             └────────┬─────────┘
                      │
                      ▼
             ┌──────────────────┐
             │ Evaluation of    │
             │ Prompt Techniques│
             └──────────────────┘


### Algorithm
Algorithm: Generative AI for Demystifying Legal Documents

Input: Legal document uploaded by the user
Output: Simplified explanation, summary, important clauses, and answers to user queries

Start
Allow the user to upload a legal document such as PDF, DOCX, or TXT.
Validate the uploaded file and extract the textual content from the document.
Perform text preprocessing by removing unnecessary spaces, symbols, and formatting while preserving the original meaning.
Divide the document into manageable sections or clauses if the document is lengthy.
Identify the user's requirement, such as:
Summarize the document
Explain a legal clause
Identify important terms
Find rights and obligations
Answer a question about the document
Select an appropriate prompting technique, such as:
Zero-shot prompting
Few-shot prompting
Role-based prompting
Step-by-step prompting
Constraint-based prompting
Construct a prompt containing the legal text and user's requirement.
Send the prompt to the Generative AI/LLM.
Analyze the generated response to identify:
Key clauses
Rights and responsibilities
Payment terms
Penalties
Dates and deadlines
Termination conditions
Potential concerns
Convert complex legal terminology into simple and understandable language without changing the original meaning.
Generate the final response in a structured format containing the summary, explanations, key points, and relevant answers.
Display the generated result to the user.
For the prompting experiment, evaluate the response using relevance, accuracy, completeness, clarity, feasibility, and usefulness.
Compare the results produced by different prompting techniques.
Identify the most effective prompting technique based on the evaluation.
Stop.

## Flowchart
                 ┌───────────────┐
                 │     START     │
                 └───────┬───────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Upload Legal        │
              │ Document            │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Validate Document   │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Extract Text from   │
              │ Document            │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Preprocess & Clean  │
              │ Extracted Text      │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Identify User       │
              │ Requirement         │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Select Prompting    │
              │ Technique           │
              └──────────┬──────────┘
                         │
                         ▼
          ┌──────────────────────────────┐
          │ Create Prompt using Legal    │
          │ Text + User Requirement       │
          └──────────────┬───────────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Generative AI /     │
              │ LLM Processing      │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Analyze Legal       │
              │ Content             │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Simplify Legal      │
              │ Language            │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Generate Summary /  │
              │ Explanation / Q&A   │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Display Results to  │
              │ User                │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Evaluate Response   │
              │ Relevance, Accuracy,│
              │ Clarity, etc.       │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Compare Prompting   │
              │ Techniques          │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Select Most         │
              │ Effective Technique │
              └──────────┬──────────┘
                         │
                         ▼
                 ┌───────────────┐
                 │      END      │
                 └───────────────┘

### For Your Prompting Experiment

You can modify the create_prompt() function and test the same legal clause using different prompting techniques:

### 1. Zero-shot
```
Explain this legal clause in simple language.
```
### 2. Role-based
```
Act as a legal document simplification assistant
and explain this clause to a non-lawyer.
```
### 3. Few-shot
```
Example:
Legal: "The tenant shall..."
Simple: "The person renting the house must..."

Now simplify the following clause:
...
```
### 4. Constraint-based
```
Explain this clause using simple English.
Use no legal jargon.
Give the answer in 3 bullet points.
Do not change the original meaning.
```

## Testing

Testing for the project “Generative AI for Demystifying Legal Documents” is performed to verify whether the system correctly processes legal documents and generates clear, accurate, and useful explanations. The same legal document can also be tested using different prompting techniques to compare their effectiveness.

### 1. Functional Testing

Functional testing checks whether each major feature works correctly.

### 2. Prompt Testing

The same legal clause is given to the AI using different prompting techniques.

### 3. Evaluation Testing

Each generated response is evaluated using a 1–5 rating scale.

### 4. Overall Testing Process

Input Legal Document → Apply Prompt → Generate AI Response → Compare with Original Document → Evaluate Response → Record Score → Compare Prompting Techniques → Identify Best Technique

### Testing Conclusion

Testing helps verify that the system can successfully extract, analyze, simplify, and explain legal documents. The prompting comparison also helps determine which technique produces the most accurate, clear, complete, and useful explanation for users without a legal background.

## Documentation
### Project Title

#### Generative AI for Demystifying Legal Documents

### 1. Introduction

Legal documents contain complex terminology, lengthy sentences, and clauses that are often difficult for people without legal knowledge to understand. The proposed system uses Generative AI to analyze legal documents and convert complicated legal language into simple and understandable explanations. It helps users identify important clauses, rights, responsibilities, penalties, dates, and other relevant information.

### 2. Objective

The main objective of the project is to develop an AI-based system that can simplify legal documents while preserving their original meaning. The project also compares different prompting techniques to identify which technique produces the most effective responses.

### 3. System Description

The system allows a user to upload a legal document. The document is processed and its text is extracted. The extracted text is provided to a Generative AI model along with a carefully designed prompt. The AI analyzes the content and generates a simplified explanation, summary, and answers to user questions.

### 4. Modules

Module 1 – Document Upload
Allows users to upload PDF, DOCX, or TXT legal documents.

Module 2 – Text Extraction
Extracts readable text from the uploaded document.

Module 3 – Text Preprocessing
Cleans and organizes the extracted text for further processing.

Module 4 – Prompt Engineering
Creates prompts using different techniques such as zero-shot, few-shot, role-based, step-by-step, and constraint-based prompting.

Module 5 – Generative AI Processing
Sends the document content and prompt to the AI model and receives the generated response.

Module 6 – Legal Document Simplification
Converts complex legal terminology into simpler language while maintaining the meaning.

Module 7 – Information Extraction
Identifies important clauses, rights, obligations, penalties, payments, dates, and termination conditions.

Module 8 – Question Answering
Allows users to ask questions about the uploaded document.

Module 9 – Evaluation
Compares responses generated using different prompting techniques based on relevance, accuracy, completeness, clarity, feasibility, and usefulness.

### 5. Limitations
AI-generated explanations may occasionally contain errors.
The system cannot replace professional legal advice.
Scanned documents may require OCR for text extraction.
Very large documents may require processing in smaller sections.
The quality of the output depends partly on the quality of the prompt and AI model.
### 6. Testing and Evaluation

The system is tested using different types of legal documents and user queries. Each prompting technique is evaluated using a 1–5 rating scale for:

Relevance, Accuracy, Completeness, Clarity, Feasibility, and Usefulness.

The results are compared to determine the prompting technique that provides the best overall performance.

### 7. Conclusion

The Generative AI for Demystifying Legal Documents system provides a practical approach for making complex legal information easier to understand. By combining document processing, prompt engineering, and Generative AI, the system can produce simplified explanations, summaries, and answers to document-related questions. The comparison of prompting techniques further helps identify how prompt design influences the quality and usefulness of AI-generated legal explanations.

## RESULT 
The prompt for the above-mentioned engineering problem was executed successfully. Different prompting techniques were applied and compared. The results demonstrated that improved prompts produced better quality, accuracy, depth, clarity and engineering usefulness than the naïve prompt. The constraint-based structured prompting technique was selected as the most effective technique, and the final refined prompt was validated through an engineering-oriented evaluation plan.
