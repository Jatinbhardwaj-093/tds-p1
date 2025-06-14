# TDS Project 1

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

TDS Project 1 is a FastAPI-based application and data preprocessing pipeline for downloading, processing, and analyzing Discourse threads. It provides a REST API to serve processed threads in JSON format.

## Project Structure

```
├── downloaded_threads/     # Raw data from Discourse API
├── markdown_files/        # Processed markdown output
├── app.py                 # FastAPI application entry point
├── preprocess.py          # Data collection and preprocessing script
├── requirements.txt       # Python dependencies
├── .env                   # Environment variables (API keys, etc.)
├── .gitignore             # Git ignore rules
├── vercel.json            # Vercel deployment configuration
├── LICENSE                # MIT License
└── README.md              # Project documentation
```

## Getting Started

1. Clone the repository:

   ```bash
   git clone https://github.com/Jatinbhardwaj-093/tds-p1.git
   cd tds-p1
   ```

2. Create a `.env` file with your Discourse API credentials:

   ```ini
   DISCOURSE_API_KEY=your_api_key
   DISCOURSE_USERNAME=your_username
   DISCOURSE_BASE_URL=https://your-discourse-instance.com
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Run data preprocessing:

   ```bash
   python preprocess.py
   ```

5. Start the FastAPI server:

   ```bash
   uvicorn app:app --reload
   ```

6. Visit `http://localhost:8000` for the welcome page.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.