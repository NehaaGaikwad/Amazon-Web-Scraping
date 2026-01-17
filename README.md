**Amazon Competitor Analysis Tool**

A Python-based market research tool that analyzes an **Amazon product** using its ASIN, scrapes competitor data, stores it locally, and generates AI-driven insights.

**Overview**

* This tool helps you perform Amazon product market research in minutes. Enter a product ASIN, and the app will automatically:

* scrape the product details

* find competitor listings

* analyze market positioning

* generate AI-driven insights and recommendations

* All results are displayed in a clean Streamlit dashboard.

**Key Features**

* Scrapes product & competitor data using Oxylabs

* Stores data locally using TinyDB

* Uses OpenAI + LangChain to generate structured insights

* Clean Streamlit UI for interactive analysis

**Outputs**

The tool generates a detailed market report including:

* Market Summary

* Product Positioning

* Competitor Comparison

* Actionable Recommendations

**How It Works**

* User enters:

        ASIN
        
        Location (Zip code)
        
        Amazon domain (e.g., amazon.com, amazon.in)

* The app scrapes:

        Main product details
        
        Competitor listings
        
        Competitor product details

* All data is stored in TinyDB.

* The formatted data is sent to OpenAI via LangChain.

* The AI generates a structured report and displays it in Streamlit.

**Ideal Use Cases**

Perfect for:

* Market research

* Product positioning analysis

* Competitor benchmarking

* Learning web scraping + LLM integration

* Portfolio or academic projects

**Tech Stack**

* Oxylabs – Real-time scraping API for Amazon product and competitor data
* requests – HTTP requests to Oxylabs
* Python scraping logic – ASIN-based scraping and competitor extraction
* TinyDB – Local JSON-based database
* os – File handling and directory creation
* datetime – Timestamping stored records
* LangChain ( ChatOpenAI , PromptTemplate , PydanticOutputParser) 
* Pydantic ( Structured AI output models (BaseModel, Field))
* dotenv ( Load API keys from .env)

