# 🧪 Test Cases – Smart Document Assistant (RAG)

## 🔹 1. Functional Tests

### TC-01: Upload PDF
- Input: Upload valid PDF
- Expected: "Processed X PDFs | Y chunks created"

### TC-02: Ask Basic Question
- Input: What is cloud computing?
- Expected:
  - Correct answer
  - Highlighted answer
  - Confidence score
  - Source displayed

### TC-03: Descriptive Question
- Input: Explain advantages of cloud computing
- Expected: Multi-line detailed answer

---

## 🔹 2. Retrieval Tests

### TC-04: Semantic Query
- Input: benefits of cloud
- Expected: Relevant answer

### TC-05: Synonym Query
- Input: uses of cloud computing
- Expected: Works correctly

### TC-06: Out-of-Scope Query
- Input: What is blockchain?
- Expected: Weak answer / fallback

---

## 🔹 3. Feature Tests

### TC-07: Confidence Score
- Expected: Value shown correctly

### TC-08: Source Citation
- Expected: Correct PDF name displayed

### TC-09: Highlighted Answer
- Expected: Only answer is highlighted

### TC-10: Export Answer
- Expected:
  - File downloads
  - Contains latest answer

---

## 🔹 4. Edge Cases

### TC-11: No PDF Uploaded
- Expected: Warning message

### TC-12: Empty Query
- Expected: No crash

### TC-13: Large PDF
- Expected: Processes successfully

---

## 🔹 5. Performance

### TC-14: Response Time
- Expected: < 5 seconds

### TC-15: Multiple Queries
- Expected: Stable performance
