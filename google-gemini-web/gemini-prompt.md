# Best Practice Prompt Examples for Gemini in Daily Chat

These examples are written for normal Gemini chat use. They are not API-style prompts. Each prompt clearly states the task, context, expected output, and simple constraints.

## 1. Explanation Prompt

```text
Explain Next.js Server Components in simple words.
I am a beginner web development student.
Please explain what they are, why they are useful, and when I should use them.
Keep the answer short and easy to understand.
```

## 2. Slide Content Prompt

```text
Help me create one simple presentation slide about Spring Boot REST API development.
The audience is beginner backend students.
Please include one title and 3 short key points.
Focus on controller, service, and repository layers.
```

## 3. Document Summary Prompt

```text
Document:
[paste the technical document about a Next.js and PostgreSQL project here]

Question:
Based on the document above, summarize the main setup steps in simple bullet points.
Only use the information from the document.
If something is not mentioned, write “Not specified.”
```

## 4. Long-Context Prompt

```text
Context:
[paste long Spring Boot project description here]

Question:
Based on the information above, what are the main weaknesses in this backend architecture?
Please suggest 3 practical improvements.
```

## 5. Multimodal Image Prompt

```text
Please analyze this system architecture diagram.
Focus on how Next.js, Spring Boot, and PostgreSQL are connected.
Tell me the main components, the data flow, the database role, and any possible architecture issues.
```

## 6. Code Debugging Prompt

```text
Error:
[paste error here]

Code:
[paste code here]

I have an error in my Spring Boot code.
Please help me find the cause and suggest the minimum fix.
Explain the problem in simple terms first.
Do not rewrite unrelated parts of the code.

```

## 7. Structured Answer Prompt

```text
Schema:
[paste PostgreSQL schema here]

Please read this PostgreSQL schema and explain its structure.
Identify the table names, primary keys, foreign keys, and relationships.
Use a clear table format if possible.

```

## 8. Translation Prompt

```text
Text:
[paste explanation here]

Please translate this technical explanation into natural academic English.
Keep the original meaning.
Do not add new information.
Make the wording clear and formal.

```

# Selected Prompt Examples for Slide

These four examples are shorter and easier to place on a slide.

## 1. Explanation Prompt

```text
Explain Next.js Server Components in simple words
I am a beginner web development student.
Please explain what they are, why they are useful, and when I should use them.
Keep the answer short and easy to understand.
```

## 2. Summarization Prompt

```text
[context]

With the technical document about a Next.js and PostgreSQL project above.
Please summarize the main setup steps in simple bullet points.
Only use the information from the document.
```

## 3. Code Debugging Prompt

```text
[code]

I have an error in my Spring Boot code.
Please help me find the cause and suggest the minimum fix.
Explain the problem in simple terms first.
```

## 4. Long-Context Prompt

```text
Context: [Paste the Spring Boot project description here]
Question: Based on the information above, what are the main backend architecture issues?
Please suggest 3 practical improvements.
```
