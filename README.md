## Tutorial 5

Name: Mirfak Naufal Pratama Putra

Class: Advance Programming B

NPM: 2306244961

<details>
<summary><b>Performance Testing Results Before And After Optimization</b></summary>

## 1. Performance Testing Results Before Optimization

### /all-student-name endpoint

#### View Results Tree
![View Results Tree for /all-student-name before optimizing](https://github.com/user-attachments/assets/2304625a-4692-4165-9770-875b153ef472)

#### View Result In Table
![View Result In Table for /all-student-name before optimizing](https://github.com/user-attachments/assets/f5d523ad-a33a-49ae-8bee-9344a3e687ff)

#### Summary Report
![Summary Report for /all-student-name before optimizing](https://github.com/user-attachments/assets/00448a5a-4ce0-4a1c-b547-9d389d566767)

#### Graph Result
![Graph Result for /all-student-name before optimizing](https://github.com/user-attachments/assets/3c25fd53-33c2-42dd-8edb-179e73e719b2)

#### CLI Test
![CLI Test for /all-student-name before optimizing](https://github.com/user-attachments/assets/7f4f8f4c-23d2-4c78-8f69-ea0e651284b3)

### /highest-gpa endpoint

#### View Results Tree
![View Result Tree for /highest-gpa before optimizing](https://github.com/user-attachments/assets/571ea100-ea2f-485a-9032-6ae509873724)

#### View Result In Table
![View Result In Table for /highest-gpa before optimizing](https://github.com/user-attachments/assets/fcb60f58-88ce-4d8d-9ef0-285d7a1022ac)

#### Summary Report
![Summary Report for /highest-gpa before optimizing](https://github.com/user-attachments/assets/34692983-8b70-4c22-9b67-226ba5113870)

#### Graph Result
![Graph Result for /highest-gpa before optimizing](https://github.com/user-attachments/assets/61ee443f-ecc5-4204-bdf2-4309b7b8581a)

#### CLI Test
![CLI Test for /highest-gpa before optimizing](https://github.com/user-attachments/assets/6e3b8f18-be03-44b8-a941-df86bd0ad9d3)

## 2. Performance Testing Results After Optimization

### /all-student-name endpoint

#### View Results Tree
![View Results Tree for /all-student-name after optimizing](https://github.com/user-attachments/assets/4a0ffcc3-316e-45ea-84df-544efea84d55)

#### View Result In Table
![View Result In Table for /all-student-name after optimizing](https://github.com/user-attachments/assets/3d09ee27-e492-404a-9cd9-86fbda13aa68)

#### Summary Report
![Summary Report for /all-student-name after optimizing](https://github.com/user-attachments/assets/4edf24d4-5f22-4e81-8034-373278d1b035)

#### Graph Result
![Graph Result for /all-student-name after optimizing](https://github.com/user-attachments/assets/b1d19c87-362d-484c-b661-c2b8b55c210a)

#### CLI Test
![CLI Test for /all-student-name after optimizing](https://github.com/user-attachments/assets/463e33cf-a103-4fb5-a202-68b4eba94caa)

### /highest-gpa endpoint

#### View Results Tree
![View Results Tree for /highest-gpa after optimizing](https://github.com/user-attachments/assets/15c7b477-11f7-4016-88b2-2e9a98857d1b)

#### View Result In Table
![View Result In Table for /highest-gpa after optimizing](https://github.com/user-attachments/assets/b41beff3-d0e2-4cc2-bd76-f06c9f736115)

#### Summary Report
![Summary Report for /highest-gpa after optimizing](https://github.com/user-attachments/assets/3607ae6d-2d2d-4374-bec1-7a7d747fcde3)

#### Graph Result
![Graph Result for /highest-gpa after optimizing](https://github.com/user-attachments/assets/586147c7-818d-4762-9085-0521083c327a)

#### CLI Test
![CLI Test for /highest-gpa after optimizing](https://github.com/user-attachments/assets/e0064b96-d52d-40a9-b444-e551958dda7a)

</details>

<details>
<summary><b>Profiling and Performance Optimization</b></summary>

#### 1. /all-student Endpoint

**Before Optimization:**
CPU Time: 805ms \
**After Optimization:**
CPU Time: 98ms \
**87.84% of improvement**
---

#### 2. /all-student-name Endpoint

**Before Optimization:** \
Average Time: 64 ms \
Min Time: 52 ms \
Max Time: 125 ms\
**After Optimization:** \
Average Time: 25 ms \
Min Time: 8 ms \
Max Time: 143 ms \
**60.94% of improvement on average time**

---

#### **3. /highest-gpa Endpoint**
**Before Optimization:** \
Average Time: 26 ms \
Min Time: 24 ms \
Max Time: 39 ms\
**After Optimization:** \
Average Time: 5 ms \
Min Time: 5 ms \
Max Time: 7 ms \
**80.77% of improvement on average time**
---
</details>

<details>
<summary><b>Reflection</b></summary>

### 1. What is the difference between the approach of performance testing with JMeter and profiling with IntelliJ Profiler in the context of optimizing application performance?
JMeter focuses on system-wide performance by simulating user loads to measure response times, throughput, and server resource usage under stress, making it ideal for identifying bottlenecks in architecture like network latency or database capacity. In contrast, IntelliJ Profiler targets code-level inefficiencies, analyzing CPU usage, memory allocation, and thread activity to pinpoint inefficient methods or memory leaks within the application. While JMeter evaluates external behavior under load, IntelliJ Profiler dives into internal operations for granular optimization.

### 2. How does the profiling process help you in identifying and understanding the weak points in your application?
Profiling identifies weak points by highlighting hotspots (methods consuming excessive resources), memory leaks, inefficient database queries, and thread contention. It provides detailed metrics on CPU usage, memory allocation, and method execution times, enabling developers to understand the root causes of inefficiencies and prioritize optimizations effectively.

### 3. Do you think IntelliJ Profiler is effective in assisting you to analyze and identify bottlenecks in your application code?
Yes, IntelliJ Profiler is highly effective, it provides real-time feedback and detailed insights into CPU, memory, and thread activity. It helps pinpoint inefficient code blocks and allows direct navigation to problematic areas, though its effectiveness depends on the developer’s ability to interpret and act on the data.

### 4. What are the main challenges you face when conducting performance testing and profiling, and how do you overcome these challenges?
Challenges:
1. Navigating around the profiling tools: This is the second time I used profiling, so it's pretty hard to navigate around.
2. Inconsistencies on profiling results: JIT compiler on the JVM is not yet optimal on the first run of the profiling test
How I overcame the challenges:
1. Getting used to the tools, once I'm used to it, it's actually not that hard
2. Repeatedly run the profiling test until I got consistent results.

### 5. What are the main benefits you gain from using IntelliJ Profiler for profiling your application code?
IntelliJ Profiler offers precision in identifying inefficient code, integrates seamlessly with IntelliJ IDEA, and provides comprehensive metrics on CPU, memory, and threads. Its real-time feedback and actionable insights make it a powerful tool for optimizing application performance efficiently.

### 6. How do you handle situations where the results from profiling with IntelliJ Profiler are not entirely consistent with findings from performance testing using JMeter?
When inconsistencies arise, cross-validate findings, focus on overlapping metrics, and re-run tests with adjusted parameters. Understand the context of each tool’s results, collaborate with team members for additional perspectives, and prioritize addressing issues that align across both tools to ensure accurate optimization.

### 7. What strategies do you implement in optimizing application code after analyzing results from performance testing and profiling? How do you ensure the changes you make do not affect the application's functionality?
Strategies: 
1. **Minimize Data Retrieval:** Fetch only required fields instead of entire objects to reduce memory usage and processing overhead.
2. **Efficient String Concatenation:** Use `String.join` or `Collectors.joining` instead of manual concatenation to avoid creating multiple intermediate `String` objects.
3. **Use Built-in Utilities:** Replace manual loops and trimming logic with optimized utilities like `Optional`, `Stream`, and `Collectors`.

**Ensuring Functionality Is Not Affected:**
**Performance Validation:** Used profiling tools to validate that optimizations achieve desired performance gains without side effects.

</details>
