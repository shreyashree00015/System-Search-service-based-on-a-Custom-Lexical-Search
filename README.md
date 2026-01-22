# System Search Service based on a Custom lexical Search
This project's code base is a part of the academic paper **_System Search Service Implementation Based on a Custom Lexical Search_** published in Procedia Computer Science. 
The paper's link: https://www.sciencedirect.com/science/article/pii/S1877050924008226

## Overview

The Intelligent Document Retrieval System is a keyword based document search application designed to retrieve files from anywhere on a user’s system based on the content inside the documents rather than just file names. The system allows users to search using generic and descriptive queries, including vernacular text, and returns relevant documents ranked by relevance.

Unlike traditional system search bars, this application indexes document contents and enables accurate content based retrieval with minimal response time after the initial indexing phase.

## Motivation

Existing system search tools are limited to retrieving files based on file names or metadata. This makes it difficult for users to locate documents when they remember the content but not the file name or location.

This project addresses that limitation by enabling content aware document retrieval, improving user efficiency and eliminating the need for manual searching across folders.

## Key Features

1. Content based document retrieval using user provided keywords
2. Support for generic and vernacular search queries
3. Relevance based ranking of retrieved documents
4. Ready to open document listing with a single click
5. Parallel processing for faster indexing and search

## Architecture

The system follows a two phase architecture:

1. Initial document indexing phase that reads and processes all documents on the system
2. Search and retrieval phase that uses the preprocessed data to return results efficiently

Parallel processing is used to divide documents into batches, reducing overall processing time and avoiding redundant file reads for each query.

## Installation

1. Clone the repository to your local machine
2. Navigate to the project root directory
3. Install the required dependencies listed in the configuration files
4. Ensure the supported document formats and system permissions are enabled

## Usage

1. Run the application to perform the initial indexing of documents
2. Enter keywords or vernacular text in the search bar
3. View the ranked list of relevant documents
4. Click on any document to open it directly

From the second run onwards, the system reuses indexed data to deliver near instant search results.

## Performance Evaluation

The system demonstrates a significant improvement in search efficiency after the initial run.

Observed performance:

1. First run indexing time approximately 303418.495 milliseconds or about 5 minutes
2. Subsequent search query time approximately 20.080 milliseconds

This optimization eliminates repeated document scanning and enables real time retrieval.

## Limitations

1. Initial indexing requires full access to document directories
2. Performance depends on system hardware and number of documents
3. Retrieval accuracy depends on document text quality and format

## Future Work

1. Support for additional document formats
2. Improved semantic search capabilities
3. Language expansion for vernacular input
4. Integration with operating system level search tools

## Contributors

This project was developed as a team with my fellow developers, Hemant(https://github.com/cvhkr19) and Pranave(https://github.com/Pranave15)
