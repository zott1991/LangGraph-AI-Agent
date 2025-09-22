# Multi-Source Research Agent

A small Python app that queries Google, Bing, and Reddit (via Bright Data datasets) and synthesizes findings.

## Requirements
- Python 3.12+
- Bright Data API key (for Reddit dataset trigger)

## Setup
1. Create/activate venv (Windows PowerShell):
   ```powershell
   python -m venv venv
   # Either bypass policy for this session, or run without activation
   Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass -Force
   .\venv\Scripts\Activate.ps1
   ```

2. Install dependencies:
   ```powershell
   .\venv\Scripts\python.exe -m pip install --upgrade pip
   .\venv\Scripts\python.exe -m pip install -r requirements.txt
   ```

3. Set environment variable:
   ```powershell
   $env:BRIGHTDATA_API_KEY = "<your_key>"
   ```
   Or create a `.env` with:
   ```
   BRIGHTDATA_API_KEY=<your_key>
   ```

## Run
```powershell
.\venv\Scripts\python.exe .\venv\main.py
```

## Notes
- If PowerShell blocks activation, call Python directly from `venv/Scripts/python.exe`.
- The Reddit search uses fallback API trigger strategies for Bright Data.
