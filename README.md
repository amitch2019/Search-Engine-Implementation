#  Multi-Strategy Search Engine Implementation

## Project Overview

This project showcases a sophisticated search engine implemented with three distinct search mechanisms, illustrating expertise in data structures, algorithms, and Python programming. The search engine processes a corpus of text files, enabling users to search for documents containing specific terms efficiently and effectively.

## Key Features

1. **Three Search Mechanisms**:
   - **Linear Search**: A straightforward search through all files, demonstrating baseline functionality.
   - **Dictionary-based Indexed Search**: Utilizes Python's built-in dictionary for fast lookup and significantly improved search speeds.
   - **Custom-implemented Hash Table**: A bespoke hash table implementation, highlighting deep understanding of hash mechanics and collision handling.

2. **Corpus Processing**: Efficiently manages large datasets, tested with a diverse range of documents including Slate magazine articles (approximately 5000) and Berlitz travelogues.

3. **Web Interface**: Displays search results in a browser, allowing users to navigate seamlessly to the original documents.

4. **Performance Comparison**: Illustrates the significant speed enhancements of indexed searches over linear search, providing a clear demonstration of the benefits of advanced data structures.

5. **HTML Generation**: Creates well-formatted HTML output for search results, including highlighted search terms for better user experience.

## Technologies Used

- **Python**: Core programming language for implementation.
- **HTML**: For generating user-friendly search results.
- **Web Browser Integration**: Utilizes the `webbrowser` module to display results.
- **HTML Templating**: Jinja2 templating engine for advanced HTML generation.

## Implementation Details

### 1. Linear Search (`linear_search.py`)
- Implements a basic linear search across all files in the corpus.
- **Time Complexity**: O(kn) for k words per file and n files.

### 2. Dict-based Indexed Search (`index_search.py`)
- Creates a fast lookup index using Python's built-in dictionary.
- **Index Creation Complexity**: O(n) for n total words in all files.
- **Search Complexity**: O(1) after indexing.

### 3. Custom Hash Table Search (`myhtable_search.py`)
- Implements a custom hash table from scratch, including custom hash function and collision handling.
- Demonstrates advanced understanding of hash table mechanics.

### 4. Main Program (`search.py`)
- Manages the user interface and search execution.
- Generates HTML output and opens results in a web browser.

## Custom Hash Table Implementation (Details)

This project includes a custom implementation of a hash table using open hashing (separate chaining) to handle collisions. The hash table is represented as a list of lists, where each bucket is a list of key-value pairs (tuples).

### Features

1. **Hash Table Creation**:
   - `htable(nbuckets)`: Initializes a hash table with a specified number of buckets, returning a list of empty lists.

2. **Hash Function**:
   - `hashcode(o)`: Computes a hash code for integers and strings. For integers, it returns the integer value directly. For strings, it calculates the hash code using a custom formula.

3. **Bucket Index Lookup**:
   - `bucket_indexof(table, key)`: Finds the index of a key within a specific bucket.

4. **Insert or Update Key-Value Pair**:
   - `htable_put(table, key, value)`: Inserts or updates the key-value pair in the appropriate bucket. If the key already exists, its value is updated. If the key does not exist, a new key-value pair is appended to the bucket.

5. **Retrieve Value by Key**:
   - `htable_get(table, key)`: Retrieves the value associated with the given key from the hash table. Returns `None` if the key is not found.

6. **Bucket String Representation**:
   - `htable_buckets_str(table)`: Returns a string representation of the hash table's buckets. Each bucket is displayed with its index and contents.

7. **Hash Table String Representation**:
   - `htable_str(table)`: Returns a string representation of the entire hash table similar to Python's dictionary `str` method. The order is based on the bucket order and the insertion order within each bucket.
   

## Challenges and Solutions

1. **Efficient Indexing**: Implemented a hash table to reduce search time from O(n) to O(1).
2. **Custom Hash Table**: Designed a robust hash function and effective collision handling mechanisms.
3. **Large Dataset Handling**: Optimized the code to process and search thousands of files efficiently.

## Future Improvements

1. Implement more advanced text processing techniques (e.g., stemming, removing stop words).
2. Add support for phrase searches and boolean operators.
3. Enhance the user interface with a more sophisticated web-based front-end.
4. Implement multi-threading for faster indexing of large corpora.

## Installation and Usage

1. **Clone the repository**:
    ```bash
    git clone https://github.com/amitch2019/multi-strategy-search-engine.git
    ```
2. **Navigate to the project directory**:
    ```bash
    cd multi-strategy-search-engine
    ```
3. **Run the search engine**:
    ```python
    python search.py
    ```
## Requirements

- Python 3.x
- Required libraries: `os`, `re`, `string`, jinja2
  
## Access to Code

- The source code for this project is **not publicly available at the moment**.
- However, it **can be shared with interested persons upon request**.
- Please contact me directly to request access to the code.

## Command Line Input

<img width="1216" alt="image" src="https://github.com/user-attachments/assets/701a4ab3-d24e-4ddd-b76b-ece94fd03839">

## Sample Output Loaded to the Default Browser

<img width="1189" alt="image" src="https://github.com/user-attachments/assets/dd6a5b62-3938-4086-91f2-d48c65ddbe78">

Contact

For any questions or inquiries, please contact me at [chaubey.amit@gmail.com].

---

This project demonstrates a robust understanding of search algorithms, data structures, and Python programming. It efficiently handles large datasets, provides significant performance improvements, and includes a user-friendly web interface for displaying search results.

