# Automated Plagiarism Detection System

## Overview
The Automated Plagiarism Detection System is a Java-based project designed to detect plagiarism between two text files. Leveraging various techniques such as tokenization, hashing, and set operations, the system efficiently identifies similarities in content and calculates a similarity score between the documents.

## Key Features
- **File Processing:** The system processes two input text files, extracting words and filtering out irrelevant characters.
- **Tokenization:** Text from each file is tokenized into individual words, allowing for precise comparison.
- **Hashing:** Hash sets are utilized to store unique words from each file, enabling fast comparison and identification of common terms.
- **Similarity Calculation:** The system computes a similarity score based on the ratio of common words to the total number of words in the documents.
- **Threshold Determination:** A configurable threshold is set to classify the similarity score as plagiarized or not plagiarized.
- **Result Reporting:** The system generates a report indicating whether plagiarism is detected between the documents and provides a confidence level based on the similarity score.

## Technologies Used
- **Java:** Core programming language used for system development.
- **File I/O:** Input/output operations for reading and processing text files.
- **Data Structures:** Utilization of hash sets for efficient storage and comparison of words.
- **Algorithms:** Implementation of set operations and similarity calculation algorithms.
- **Error Handling:** Incorporation of exception handling mechanisms to manage file-related errors.

## Usage
1. **Input:** Place the text files to be compared in the same directory as the Java program.
2. **Execution:** Compile and run the Java program specifying the filenames as command-line arguments.
   ```
   javac Main.java
   java Main file1.txt file2.txt
   ```
3. **Output:** The system will display the similarity score and a classification indicating whether plagiarism is detected.

## Runtime Efficiency
- **Runtime Complexity:** The system operates with a time complexity of O(n) for processing each file, where n is the number of words in the file. The overall time complexity for comparing two files is O(n^2), considering the comparison of each word from one file with every word in the other file.
- **Space Complexity:** The space complexity of the system is O(n), where n is the total number of unique words across both files. The usage of hash sets allows for efficient storage and retrieval of words, minimizing memory consumption.

## Future Enhancements
- **Enhanced User Interface:** Develop a user-friendly interface for easy interaction and result visualization.
- **Integration with Version Control Systems:** Enable integration with version control platforms to analyze changes in document content over time.
- **Machine Learning Integration:** Implement machine learning models to enhance plagiarism detection accuracy and adaptability.
- **Cross-Language Support:** Extend the system to support detection across multiple languages, catering to diverse user requirements.
- **Real-Time Monitoring:** Implement real-time monitoring capabilities to detect plagiarism as new documents are added to the system.

## Conclusion
The Automated Plagiarism Detection System offers a robust solution for identifying plagiarized content, contributing to academic integrity, intellectual property protection, and content quality assurance. With its scalable architecture and advanced features, the system serves as a valuable tool for organizations and individuals seeking to maintain originality and uphold ethical standards in content creation and dissemination.
