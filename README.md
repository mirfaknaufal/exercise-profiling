## Tutorial 5

Name: Mirfak Naufal Pratama Putra

Class: Advance Programming B

NPM: 2306244961

<details>
<summary><b>Performance Testing Results Before And After Optimization</b></summary>

## 1. Performance Testing Results Before Optimization

### /all-student-name endpoint

#### View Results Tree

#### View Result In Table

#### Summary Report

#### CLI Test

### /highest-gpa endpoint

#### View Results Tree

#### View Result In Table

#### Summary Report

#### CLI Test

## 2. Performance Testing Results After Optimization

### /all-student-name endpoint

#### View Results Tree

#### View Result In Table

#### Summary Report

#### CLI Test

### /highest-gpa endpoint

#### View Results Tree

#### View Result In Table

#### Summary Report

#### CLI Test
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
#### JMeter focuses on system-wide performance by simulating user loads to measure response times, throughput, and server resource usage under stress, making it ideal for identifying bottlenecks in architecture like network latency or database capacity. In contrast, IntelliJ Profiler targets code-level inefficiencies, analyzing CPU usage, memory allocation, and thread activity to pinpoint inefficient methods or memory leaks within the application. While JMeter evaluates external behavior under load, IntelliJ Profiler dives into internal operations for granular optimization.

### 2. How does the profiling process help you in identifying and understanding the weak points in your application?
#### Profiling identifies weak points by highlighting hotspots (methods consuming excessive resources), memory leaks, inefficient database queries, and thread contention. It provides detailed metrics on CPU usage, memory allocation, and method execution times, enabling developers to understand the root causes of inefficiencies and prioritize optimizations effectively.

### 3. Do you think IntelliJ Profiler is effective in assisting you to analyze and identify bottlenecks in your application code?
#### Yes, IntelliJ Profiler is highly effective, it provides real-time feedback and detailed insights into CPU, memory, and thread activity. It helps pinpoint inefficient code blocks and allows direct navigation to problematic areas, though its effectiveness depends on the developer’s ability to interpret and act on the data.

### 4. What are the main challenges you face when conducting performance testing and profiling, and how do you overcome these challenges?
#### Challenges:
#### 1. Navigating around the profiling tools: This is the second time I used profiling, so it's pretty hard to navigate around.
#### 2. Inconsistencies on profiling results: JIT compiler on the JVM is not yet optimal on the first run of the profiling test
#### How I overcame the challenges:
#### 1. Getting used to the tools, once I'm used to it, it's actually not that hard
#### 2. Repeatedly run the profiling test until I got consistent results.

### 5. What are the main benefits you gain from using IntelliJ Profiler for profiling your application code?
#### IntelliJ Profiler offers precision in identifying inefficient code, integrates seamlessly with IntelliJ IDEA, and provides comprehensive metrics on CPU, memory, and threads. Its real-time feedback and actionable insights make it a powerful tool for optimizing application performance efficiently.

### 6. How do you handle situations where the results from profiling with IntelliJ Profiler are not entirely consistent with findings from performance testing using JMeter?
#### When inconsistencies arise, cross-validate findings, focus on overlapping metrics, and re-run tests with adjusted parameters. Understand the context of each tool’s results, collaborate with team members for additional perspectives, and prioritize addressing issues that align across both tools to ensure accurate optimization.

### 7. What strategies do you implement in optimizing application code after analyzing results from performance testing and profiling? How do you ensure the changes you make do not affect the application's functionality?
#### Strategies: 
#### 1. **Minimize Data Retrieval:** Fetch only required fields instead of entire objects to reduce memory usage and processing overhead.
#### 2. **Efficient String Concatenation:** Use `String.join` or `Collectors.joining` instead of manual concatenation to avoid creating multiple intermediate `String` objects.
#### 3. **Use Built-in Utilities:** Replace manual loops and trimming logic with optimized utilities like `Optional`, `Stream`, and `Collectors`.

#### Ensuring Functionality Is Not Affected:
####  **Performance Validation:** Used profiling tools to validate that optimizations achieve desired performance gains without side effects.

</details>