# Python Virtual Environment Setup Guide

## Virtual Environment Created Successfully! ✅

Your Python virtual environment has been created in the `venv` directory.

## How to Activate the Virtual Environment

### Method 1: Using Batch File (Recommended for Windows)
```cmd
venv\Scripts\activate.bat
```

### Method 2: Manual Environment Setup (PowerShell)
```powershell
$env:VIRTUAL_ENV = "C:\Users\zotto\Documents\TwtProject\venv"
$env:PATH = "C:\Users\zotto\Documents\TwtProject\venv\Scripts;$env:PATH"
```

### Method 3: PowerShell Script (if execution policy allows)
```powershell
.\venv\Scripts\Activate.ps1
```

## Verify Activation
After activation, you should see:
- Python executable pointing to: `C:\Users\zotto\Documents\TwtProject\venv\Scripts\python.exe`
- Virtual environment prefix: `C:\Users\zotto\Documents\TwtProject\venv`

## How to Deactivate
Simply run:
```cmd
deactivate
```

## Installing Packages
Once activated, you can install packages using:
```cmd
python -m pip install package_name
```

## Notes
- The virtual environment is isolated from your system Python
- All packages installed will be contained within this environment
- Remember to activate the environment each time you work on your project

