# itsm-human-factors
Research on human factors in ITSM implementation with API-driven data analysis
# The Human Element of ITSM: Research in Progress

[![Research Status](https://img.shields.io/badge/Status-In%20Progress-brightgreen)](https://github.com/yourusername/itsm-human-factors)

## Research Hypothesis
The successful implementation and business value realization of IT Service Management frameworks depends significantly on human factors such as role clarity, burnout prevention, and organizational commitment, beyond the technical and process-oriented aspects traditionally emphasized in ITSM literature.

## API-Driven Research Approach
This research leverages several APIs to analyze ITSM literature and extract insights:

- Academic Literature APIs for paper retrieval
- Natural Language Processing APIs for thematic analysis
- Data Visualization APIs for pattern identification

## Current Progress
- ✅ Initial literature collection and processing via API
- ✅ Thematic analysis of 47 ITSM documents completed
- 🔄 Development of data extraction pipeline
- 📅 Survey design and distribution (Upcoming)

## Technical Implementation
The current focus is on developing the theme extraction pipeline using NLP Cloud and other APIs:

```python
def extract_themes_from_text(text, api_key):
    """Extract themes from text using NLP API."""
    url = "https://api.nlpcloud.io/v1/bart-large/summarization"
    
    headers = {
        "Authorization": f"Token {api_key}",
        "Content-Type": "application/json"
    }
    
    payload = {"text": text, "min_length": 30, "max_length": 100}
    response = requests.post(url, headers=headers, json=payload)
    
    # Process API response...
