# AdVibe-Context-Based-Ad-Recommendation-System
Privacy-Friendly, Real-Time Ad Suggestions Using Google Gemini API and Web Scraping.


## Overview

AdVibe extracts content from web pages, analyzes it using Google's Gemini AI, and generates relevant advertising categories. This can be useful for:

- Content creators looking to monetize their websites
- Marketers seeking to improve ad targeting
- Developers building contextual advertising solutions

## Features

- 🌐 Web content extraction using BeautifulSoup
- 🧠 Content analysis with Google's Gemini AI
- 🎯 Generation of context-relevant ad categories
- 📊 Simple display of recommended ad categories

## Prerequisites

- Python 3.7+
- Google API key for Gemini AI

## Installation

1. Clone this repository:
```
git clone https://github.com/DPRASAD-dp/AdVibe-Context-Based-Ad-Recommendation-System.git
cd AdVibe: Context-Based Ad Recommendation System
```

2. Install required packages:
```
pip install google-generativeai beautifulsoup4 requests python-dotenv
pip install -U google-generativeai
```

## Setup

There are two ways to configure your Google API key:

### Option 1: Environment Variables (Recommended)
1. Create a `.env` file in the project root:
```
GOOGLE_API_KEY=your_api_key_here
```

2. Load the environment variable in your code:
```python
from dotenv import load_dotenv
load_dotenv()
api_key = os.getenv("GOOGLE_API_KEY")
```

### Option 2: Direct API Key (Not recommended for production)
```python
api_key = "your_api_key_here"
```

## Usage

```python
# Import the module
from advibe import run_ad_system

# Run the system on a specific URL
run_ad_system("https://www.example.com/article")
```

## Example

```python
test_url = "https://www.bbc.com/sport/cricket/articles/cly2l3j6ev2o"
run_ad_system(test_url)
```

Output:
```
🚀 Extracting content from: https://www.bbc.com/sport/cricket/articles/cly2l3j6ev2o
🔍 Analyzing content with Gemini API...
✅ Generated Categories: 
1. Sports Streaming Services/Apps
2. Sports News & Media
3. Travel & Tourism (India & Cricket Locations)
4. Sportswear & Equipment (Cricket Specific)
5. Fantasy Sports & Online Betting


```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- [Google Generative AI](https://ai.google.dev/)
- [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/)
