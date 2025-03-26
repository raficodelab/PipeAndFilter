# PipeAndFilter Pattern

## Overview
This project demonstrates the **Pipe and Filter** architectural pattern using Java. The implementation applies a sequence of transformations (filters) to an input list of integers, processing them step by step.

## Features
- Filters even numbers
- Squares the numbers
- Filters numbers greater than 10
- Removes numbers less than 5

## Technologies Used
- Java 8+
- Java Streams API

## How It Works
The pipeline consists of multiple filters, applied sequentially:
1. **Filter even numbers**: Removes odd numbers from the list.
2. **Square numbers**: Computes the square of each number.
3. **Filter numbers greater than 10**: Retains only numbers greater than 10.
4. **Filter numbers less than 5**: Retains only numbers greater than or equal to 5.

The filters are stored as `Function<List<Integer>, List<Integer>>` and applied in sequence.

## Code Structure
- **`processPipeline`**: Applies the filters in order.
- **Filter Methods**:
  - `filterEvenNumbers(List<Integer>)`
  - `squareNumbers(List<Integer>)`
  - `filterNumbersGreaterThanTen(List<Integer>)`
  - `filterNumbersLessThanFive(List<Integer>)`

## Usage
Compile and run the Java program:
```sh
javac PipeAndFilter.java
java PipeAndFilter
```

## Example Output
```sh
[16, 36, 64, 100]
```

## License
This project is open-source under the MIT License.

