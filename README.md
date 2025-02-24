# BROCHURE BUILDER

## Overview
Brochure Builder is a Python tool that extracts relevant content from a company website and generates a concise brochure using OpenAI's GPT model. The brochure is tailored for potential customers, investors, and job seekers.

## Features
- Scrapes webpage content and extracts key information.
- Identifies important links related to company information, careers, and about pages.
- Uses OpenAI's GPT model to generate a well-structured markdown brochure.
- Filters out irrelevant links such as privacy policies and terms of service.

## Installation
Ensure you have Python 3.10+ installed, then install the required dependencies:
```sh
pip install requests dotenv beautifulSoup4 openai
```

## Usage
1. Set up your OpenAI API key in a `.env` file:
```
OPENAI_API_KEY=your_openai_api_key_here
```

2. Import and run the script:
```python
from brochure_builder import create_brochure

create_brochure('CompanyName', 'https://www.companywebsite.com')
```

## How It Works
1. **Website Scraping:**
   - Fetches the webpage content and extracts text while removing scripts, images, and styles.
   - Collects relevant links for about pages, careers, and company information.
   
2. **AI-Powered Content Processing:**
   - Sends the extracted data to OpenAI's GPT model.
   - Generates a markdown-format brochure summarizing the company's details.
   
3. **Brochure Output:**
   - Displays the generated brochure in markdown format.
   

## Dependencies
- Python 3.10+
- `requests`
- `dotenv`
- `beautifulSoup4`
- `openai`



## Author
Developed by Sidharth Rana.

