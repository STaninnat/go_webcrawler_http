# Web Crawler

This project is a web crawler built from scratch in Go. It's designed as an SEO analytics tool that reports on the internal linking profile of any website. By making HTTP requests and parsing HTML, the crawler generates reports that SEO experts can use to analyze a website's internal structure. The report can be marshaled to standard output or written to a file for further analysis.

## Features

- **Web Crawling**: Traverse and crawl websites to gather internal linking information.
- **HTML Parsing**: Extract links and relevant data from web pages by parsing HTML.
- **Command-Line Interface**: A Go-based CLI application that runs the crawler and outputs results.
- **Flexible Output**: Reports can be printed directly to the console or written to a file for later review.

## Tools and Libraries

- **Go**: The core programming language used for building the web crawler.
- **net/http**: Go's standard library for making HTTP requests.
- **golang.org/x/net/html**: Go's library for parsing HTML documents.
- **os and io packages**: For handling file output and command-line operations.

## How to Run

1. Clone the repository.
2. Ensure you have Go installed on your system with ```go version```
3. Run the web crawler with the following command: 
    `go build -o crawler`
    `./crawler URL maxConcurrency maxPages **Example: ./crawler "https://example.com" 3 10**`
    - *```go build``` and ```./crawler``` can also be replaced with ```go run .``` from your main package directory.*
