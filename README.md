# CAD-to-BOM-Generator
AI-powered CAD Bill of Materials generator with real component extraction"
# CAD Bill of Materials (BoM) Generator
<img width="1874" height="743" alt="Screenshot 2025-10-01 173312" src="https://github.com/user-attachments/assets/266b86d1-ebed-47c6-930a-94482124761c" />
<img width="1851" height="714" alt="Screenshot 2025-10-01 173324" src="https://github.com/user-attachments/assets/80636bab-0ef0-4036-8d63-541010eb20e5" />
<img width="1833" height="733" alt="Screenshot 2025-10-01 173338" src="https://github.com/user-attachments/assets/ec5c47ab-b8cc-4fde-9816-7d0ab09cb889" />
<img width="1829" height="708" alt="Screenshot 2025-10-01 173351" src="https://github.com/user-attachments/assets/8c16aab9-72b4-4aaa-8920-828fa3556876" />

[![Python](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.104.1-green.svg)](https://fastapi.tiangolo.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

An AI-powered tool for automatically generating detailed Bill of Materials from CAD files. Extracts real component specifications, dimensions, and materials to create professional construction estimates.

[cad-bom-generator.zip (1).zip](https://github.com/user-attachments/files/22636990/cad-bom-generator.zip.1.zip)


## 🌟 Features

- **🔧 Advanced CAD Processing**: Support for DXF, DWG, and PDF files
- **🤖 Intelligent Component Detection**: AI-powered symbol recognition and specification extraction  
- **📏 Real Dimension Extraction**: Actual measurements from CAD geometry
- **🏗️ Material Identification**: Automatic detection of materials and finishes
- **📊 Professional BoM Generation**: Multi-format export with detailed analysis
- **⚠️ Empty File Detection**: Proper handling of empty or invalid files
- **🌐 Web Interface**: Modern, responsive UI for easy interaction

## 🚀 Quick Start

### Installation

1. **Clone the repository:**
```bash
git clone https://github.com/yourusername/cad-bom-generator.git
cd cad-bom-generator
```

2. **Create virtual environment:**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies:**
```bash
pip install -r requirements.txt
```

4. **Run the application:**
```bash
python main.py
```

5. **Open your browser to:** `http://localhost:8000`

### Usage

1. **📁 Upload CAD File**: Drag and drop your DXF, DWG, or PDF file
2. **🔍 Review Analysis**: Check detected components and specifications  
3. **📋 Generate BoM**: Create detailed Bill of Materials with real measurements
4. **📊 Export Results**: Download professional Excel reports with analysis

## 📊 Example Output

| Item | Description | Qty | Unit | Dimensions | Material | Unit Cost | Total Cost |
|------|-------------|-----|------|------------|----------|-----------|------------|
| 001 | Steel Entry Door 36" × 84" | 2 | each | 36×84 | Steel | $850.00 | $1,700.00 |
| 002 | Aluminum Window 48" × 60" | 6 | each | 48×60 | Aluminum | $425.00 | $2,550.00 |
| 003 | 20A GFCI Duplex Receptacle | 15 | each | Standard | Plastic | $35.00 | $525.00 |
| | | | | | **TOTAL COST** | | **$4,775.00** |

## 🛠️ Development

### Running Tests
```bash
pytest tests/
```

### API Documentation
- **Swagger UI**: `http://localhost:8000/docs`
- **ReDoc**: `http://localhost:8000/redoc`

### Project Structure
```
cad-bom-generator/
├── src/                    # Core processing modules
├── api/                    # FastAPI backend
├── web/                    # Frontend interface
├── tests/                  # Test suite
├── docs/                   # Documentation
└── examples/               # Usage examples
```

## 🔧 API Endpoints

| Endpoint | Method | Description |
|----------|--------|-------------|
| `/api/upload-enhanced` | POST | Upload CAD files with comprehensive processing |
| `/api/analysis/{task_id}` | GET | Get detailed CAD analysis results |
| `/api/components/{task_id}` | GET | Get extracted components with specifications |
| `/api/generate-detailed-bom/{task_id}` | POST | Generate comprehensive BoM |
| `/api/export-comprehensive/{task_id}` | POST | Export detailed Excel reports |

## 🤝 Contributing

1. Fork the repository
2. Create feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built for the construction industry
- Powered by FastAPI and modern web technologies



---

⭐ **Star this repository if it helped you!** ⭐
