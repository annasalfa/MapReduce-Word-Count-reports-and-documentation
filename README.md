# MapReduce Word Count Implementation (Ubuntu on DigitalOcean)

## 📘 English Version

### Overview
This project demonstrates the implementation of the **MapReduce** programming model for counting word frequency using **Apache Hadoop** on **Ubuntu 18.04** deployed through **DigitalOcean**.

The purpose of this implementation is to analyze distributed data processing by parallelizing a simple word counting task, showcasing the efficiency of MapReduce in handling large text datasets.

### Environment & Tools
- Ubuntu 18.04 (DigitalOcean Droplet)
- Java Development Kit (JDK)
- Apache Hadoop Framework

### Steps Summary
1. Connect to the Ubuntu droplet via SSH.
2. Prepare input and output folders (`input`, `output`).
3. Create a Java file `WordCount.java` containing the Mapper and Reducer logic.
4. Compile the Java code using Hadoop’s classpath:
   ```bash
   javac -classpath $HADOOP_CLASSPATH -d bin/ WordCount.java
   ```
5. Package it as a JAR file and execute it with:
   ```bash
   hadoop jar WordCount.jar WordCount input output
   ```
6. Output results are stored in:
   ```bash
   output/part-r-00000
   ```

### Result
The program successfully counts and aggregates word frequencies from an input text file (e.g., a novel).

This demonstrates the parallel processing power of the MapReduce framework.

### Author

**Annas Al Farisi**

Cloud Developer, MLOps & Automation Enthusiast

📧 Email: annasalfarisi@gmail.com

🔗 GitHub: https://github.com/annasalfa

💼 LinkedIn: https://linkedin.com/in/annasalfa

### License

MIT License © 2025 Annas Al Farisi

Free for personal, academic, and educational use.