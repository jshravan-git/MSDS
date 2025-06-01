
# Fine-Tuning a GPT Model

## Author
**Saravanan Janarthanan**

## Project Overview

This milestone demonstrates the process of **fine-tuning an OpenAI model** using a domain-specific dataset involving chicken recipes. The goal is to guide the model to respond contextually based on provided examples, improving its relevance and accuracy in a specific use case.

---

## Objectives

- Structure conversational data in `JSONL` format
- Validate the format and estimate token usage
- Upload the dataset and trigger the fine-tuning process using OpenAI API
- Use the fine-tuned model for domain-specific inference

---

## Fine-Tuning Workflow

### Step 1: Create a JSONL Dataset
Each entry in the file is a conversation turn:
```json
{
  "messages": [
    {"role": "system", "content": "You provide chicken recipes from a given list."},
    {"role": "user", "content": "Give me a recipe for chicken Meatloaf"},
    {"role": "assistant", "content": "Recipe Name: Chicken Meatloaf..."}
  ]
}
```

### Step 2: Validate JSONL Format
- Ensure required keys like `role` and `content` exist
- Verify roles are among `system`, `user`, `assistant`, or `function`
- Catch and report errors during validation

### Step 3: Estimate Token Count
- Use the **tiktoken** module to simulate OpenAI’s tokenizer
- Calculate total tokens per message
- Ensure data size fits within fine-tuning constraints

### Step 4: Upload JSONL for Fine-Tuning
- Upload using OpenAI API with `purpose="fine-tune"`
- Get a file ID after successful upload and processing

### Step 5: Start Fine-Tuning
- Use the file ID and base model (`gpt-4o-mini-2024-07-18`)
- Track job status using a job ID
- Wait for `succeeded` status to confirm completion

### Step 6: Use the Fine-Tuned Model
- Use the new model name for inference
- Structure prompts with `system` and `user` messages
- Generate context-aware chicken recipe responses

---

## Technologies Used

- **Python**
- **OpenAI API**
- **tiktoken** (for token analysis)
- **JSON / JSONL**
- **Defaultdict & Exception Handling** (for robust validation)

---

## Usage

1. Set up the environment:
```bash
pip install openai tiktoken
```

2. Store your OpenAI API key in a local `.txt` file.

3. Run the notebook step-by-step to:
   - Validate the JSONL data
   - Check token limits
   - Upload the file and start fine-tuning
   - Query the fine-tuned model
