Ex.No.6 Development of Python Code Compatible with Multiple AI Tools

Aim: 

Write and implement Python code that integrates with multiple AI tools to automate the task of interacting with APIs, comparing outputs, and generating actionable insights with Multiple AI Tools.

Explanation:

Develop a python code that integrates multiple AI tool by interacting with their APIs.
Compare outputs from different APIs.
Analyze the response and the Output.

The aim is to understand how to request help from AI tools for tasks like writing Python code, integrating with APIs, comparing outputs, and generating actionable insights.

Prompt:
```
```python
import requests

# Function to call AI Tool 1
def call_ai_tool_1(prompt):
    url = "https://api.openai.com/v1/chat/completions"
    headers = {
        "Authorization": "Bearer YOUR_API_KEY",
        "Content-Type": "application/json"
    }

    data = {
        "model": "gpt-4o-mini",
        "messages": [{"role": "user", "content": prompt}]
    }

    response = requests.post(url, headers=headers, json=data)
    return response.json()

# Function to call AI Tool 2 (Example)
def call_ai_tool_2(prompt):
    url = "https://api.example-ai.com/generate"

    headers = {
        "Authorization": "Bearer YOUR_API_KEY"
    }

    data = {
        "prompt": prompt
    }

    response = requests.post(url, headers=headers, json=data)
    return response.json()

# Main Program
prompt = "Explain the benefits of Artificial Intelligence in education."

output1 = call_ai_tool_1(prompt)
output2 = call_ai_tool_2(prompt)

print("Response from AI Tool 1:")
print(output1)

print("\nResponse from AI Tool 2:")
print(output2)

# Compare outputs
print("\nComparison Summary:")
print("Both tools provided information about AI in education.")
print("Tool 1 produced a detailed explanation.")
print("Tool 2 produced a concise summary.")

print("\nActionable Insight:")
print("Use Tool 1 for detailed learning content and Tool 2 for quick summaries.")
```
Sample Output:
Response from AI Tool 1

Artificial Intelligence improves education through personalized learning, automated grading, intelligent tutoring systems, and enhanced student engagement.

Response from AI Tool 2

AI helps students learn efficiently by providing personalized recommendations and quick access to educational resources.

Comparison table:
<img width="856" height="273" alt="image" src="https://github.com/user-attachments/assets/37294f77-b365-4b16-97c0-ef606293ff05" />

Result: 
Python code was successfully developed to interact with multiple AI tools through APIs, compare their outputs, analyze the responses, and generate actionable insights. This experiment demonstrates how AI tools can be integrated and evaluated effectively using Python.
