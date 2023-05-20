# GeoScout

This repository contains a web crawler built in Python. The crawler is designed to extract data from websites by recursively traversing links and scraping relevant information.

## Features

- **Website crawling:** The crawler can start from a given URL and follow links to crawl multiple pages.
- **Data extraction:** It extracts desired data from the crawled web pages using customizable scraping rules.
- **Parallel processing:** The crawler supports concurrent processing to improve performance.
- **Robustness:** It handles common web crawling challenges like handling different types of content, avoiding duplicate URLs, and respecting the site's robots.txt file.

## Getting Started

### Prerequisites

- Java and Spring Boot

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/web-crawler.git
   
## Microservices

### Crawler (Includes a Crawler and a Scrapper)

## ScoutDB

- scout_id (number) : unique primary key (not null)
- url (string) : internal urls (not null)
- status_code (number): state (not null with constraints) (501 - Pending, 502 - Completed) 

## Phase 1

- Effectively download all the internal urls and store in ScoutDB. Set status code to 501. 
- Maintain the crawler (re-crawl latest data)
- A flag to track whether its is crawled for the first time. (in application configurations)

