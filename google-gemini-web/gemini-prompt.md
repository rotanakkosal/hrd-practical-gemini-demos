# Best Practice Prompt Examples for Gemini

## 1. Explanation Prompt

```text
Explain Next.js server-side rendering to beginner web development students.
Use simple and connected sentences.
Focus on what SSR is, why it is useful, and when developers should use it.
Avoid deep technical terms.
Return the answer in 2 short paragraphs.
```

## 2. Slide Content Prompt

```text
Create one presentation slide about Spring Boot REST API development.
The audience is beginner backend students.
Use short, clear sentences.
Include one title and 3 key points.
Focus on controller, service, and repository layers.
Keep the tone simple and academic.
```

## 3. Document Summary Prompt

```text
Based on the technical document below, summarize the main setup steps for a Next.js and PostgreSQL project.
Only use information from the document.
If something is not mentioned, write “Not specified.”
Keep each bullet point under 20 words.
Document: [paste document]
```

## 4. Long-Context Prompt

```text
Read the full context below first.
After reading it, answer the question at the end.
Base your answer only on the provided context.
If evidence is missing, say clearly that the context does not provide enough information.
Context: [paste long Spring Boot project description]
Question: Based on the information above, what are the main weaknesses in this backend architecture?
```

## 5. Multimodal Image Prompt

```text
Analyze the attached system architecture diagram.
Identify the main components, data flow, and database connection.
Focus on how Next.js, Spring Boot, and PostgreSQL interact.
Return the answer in this format:
1. Main components
2. Data flow
3. Database role
4. Possible architecture issues
```

## 6. Code Debugging Prompt

```text
You are a Spring Boot debugging assistant.
Find the cause of this error and suggest the minimum fix.
Explain the problem in simple terms first, then provide the corrected code.
Do not rewrite unrelated parts of the code.
Error: [paste error]
Code: [paste Spring Boot code]
```

## 7. Structured Output Prompt

```text
Extract the following information from the SQL schema: table names, primary keys, foreign keys, and relationships.
Return valid JSON only.
If a field is missing, use null.
SQL schema: [paste PostgreSQL schema]
```

## 8. Translation Prompt

```text
Translate the following technical explanation into natural academic English.
Preserve the original meaning.
Do not add new information.
Use clear and formal wording.
Text: [paste explanation about Next.js, Spring Boot, or PostgreSQL]
```
