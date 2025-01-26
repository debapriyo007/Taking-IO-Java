# Competitive Programming Solution In Java



This repository contains a Java program designed for competitive programming. It provides a basic structure for efficiently handling input and output using custom classes (`InputReader` and `OutputWriter`) to streamline the problem-solving process during contests.

## Table of Contents

| Coding Platform                                                                                       |  Accepted |
|---------------------------------------------------------------------------------------------|-----------------|
| ![CodeChef](https://img.shields.io/badge/CodeChef-%23964B00.svg?style=for-the-badge&logo=CodeChef&logoColor=white) | ✅ Yes          |
| ![Codeforces](https://img.shields.io/badge/Codeforces-445f9d?style=for-the-badge&logo=Codeforces&logoColor=white) | ✅ Yes          |




## Features

- **Custom Input Handling:**
  - `InputReader` supports efficient reading of various data types such as `int`, `long`, `double`, and strings.
  - Supports reading lines for custom input scenarios.

- **Custom Output Handling:**
  - `OutputWriter` enables fast and efficient output.
  - Provides methods to write and writeLine for better control over the output.

- **Error Handling:**
  - Includes runtime exception handling for input/output operations.


## Usage

- Copy the bellow code and use it for competitive programming.
- Accepted in any competitive programming platform.

### Boilerplate Code

```java
import java.util.*;
import java.io.*;

public class CompetitiveProgrammingSolution {

    static class InputReader {
        private BufferedReader reader;
        private StringTokenizer tokenizer;

        public InputReader() {
            reader = new BufferedReader(new InputStreamReader(System.in));
        }

        public String next() {
            while (tokenizer == null || !tokenizer.hasMoreTokens()) {
                try {
                    tokenizer = new StringTokenizer(reader.readLine());
                } catch (IOException e) {
                    throw new RuntimeException("Error reading input", e);
                }
            }
            return tokenizer.nextToken();
        }

        public int nextInt() {
            return Integer.parseInt(next());
        }

        public long nextLong() {
            return Long.parseLong(next());
        }

        public double nextDouble() {
            return Double.parseDouble(next());
        }

        public String readLine() {
            String inputLine = "";
            try {
                inputLine = reader.readLine();
            } catch (IOException e) {
                throw new RuntimeException("Error reading line", e);
            }
            return inputLine;
        }
    }

    static class OutputWriter {
        private BufferedWriter writer;

        public OutputWriter() {
            writer = new BufferedWriter(new OutputStreamWriter(System.out));
        }

        public void write(Object object) throws IOException {
            writer.write(object.toString());
        }

        public void writeLine(Object object) throws IOException {
            write(object);
            writer.newLine();
        }

        public void close() throws IOException {
            writer.close();
        }
    }

    public static void main(String[] args) {
        try {
            InputReader inputReader = new InputReader();
            OutputWriter outputWriter = new OutputWriter();

            int T = inputReader.nextInt();
            while (T -- > 0) {
               
               // Solve the problem here
               // Call the solveProblem method.
            }
            outputWriter.close();
        } catch (Exception e) {
            System.err.println("Error during program execution: " + e.getMessage());
        }
    }

}
```

1. **InputReader**: Handles reading input from the standard input.
2. **OutputWriter**: Handles writing output to the standard output.
3. **solveProblem**: The main logic for solving the competitive programming problem goes here.



## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Java community for the efficient `BufferedReader` and `BufferedWriter` classes.
- Inspiration from competitive programming contests such as Codeforces, LeetCode, and HackerRank.

<p align="center">
    <img src="https://media2.giphy.com/media/3O5Ae20Rc0yuzlAroL/200w.gif?cid=82a1493bheh8va1kfb4wgpkqkineb4gznte8i2vwtdwpqg8g&ep=v1_gifs_related&rid=200w.gif&ct=s" alt="alt text">
</p>


