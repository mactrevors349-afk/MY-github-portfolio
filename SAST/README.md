# 🔒 Security & SAST Projects

Welcome to the Security & Tooling section of my portfolio. This folder contains projects focused on application security, vulnerability detection, and secure coding practices.

---

## 🔒 PyCodeScan - Python SAST Security Analysis Tool

**Repository:** [PyCodeScan](https://github.com/mactrevors349-afk/PyCodeScan)

### 📋 Project Overview
A Python-based **Static Application Security Testing (SAST)** tool designed to identify security vulnerabilities and insecure coding patterns in Python source code. PyCodeScan performs line-by-line analysis to detect common security anti-patterns before code is deployed, making it ideal for developers using VS Code or similar IDEs who want a lightweight, fast security scan.

### 🔑 Key Features
- 🛡️ **Arbitrary Code Execution Detection**: Identifies risky patterns like `eval()`, `os.system()`, and unsafe `subprocess.run()` calls
- 🔐 **Insecure Deserialization Scanning**: Flags dangerous functions like `pickle.loads()` and `yaml.load()`
- ⚠️ **Sensitive Data Exposure**: Detects hardcoded credentials (passwords, API keys)
- 🔍 **Input Validation Analysis**: Highlights unsanitized user input vulnerabilities
- 📊 **Line-by-Line Reporting**: Detailed console output with line numbers and vulnerable code snippets
- ⚡ **Lightweight & Fast**: Quick scanning ideal for local development workflows
- 🎯 **Educational & Practical**: Built for developers learning security best practices

### 🛠️ Technologies Used
- **Language:** Python
- **Core Technology:** Pattern-based string matching and lexical analysis
- **I/O:** File handling and console-based reporting
- **Focus Areas:** SAST, Code vulnerability detection, Developer security education

### 📂 Project Architecture
```
PyCodeScan/
├── vulnerabilityscanner.py    # Core SAST engine
├── insecure_patterns/         # Vulnerability pattern definitions
├── reports/                   # Scan output formatting
├── tests/                     # Test cases
└── README.md                  # Documentation
```

### 🚀 Getting Started
To use PyCodeScan:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/mactrevors349-afk/PyCodeScan.git
   cd PyCodeScan
   ```

2. **Run a security scan:**
   ```bash
   python vulnerabilityscanner.py /path/to/python/file.py
   ```

3. **Scan entire directory:**
   ```bash
   python vulnerabilityscanner.py /path/to/project/
   ```

4. **View detailed results:**
   - Line numbers with vulnerable patterns
   - Severity level and vulnerability description
   - Code snippet context
   - Remediation recommendations

### 🔗 Live Links
- **GitHub Repository:** [mactrevors349-afk/PyCodeScan](https://github.com/mactrevors349-afk/PyCodeScan)
- **View Code:** [PyCodeScan repository on GitHub](https://github.com/mactrevors349-afk/PyCodeScan/tree/main)

### 📚 Detected Vulnerability Categories

#### 1. **Arbitrary Code Execution**
- `eval()` function usage
- `os.system()` shell command execution
- Unsafe `subprocess.run()` with `shell=True`

#### 2. **Insecure Deserialization**
- `pickle.loads()` on untrusted data
- `yaml.load()` (recommends `yaml.safe_load()`)

#### 3. **Sensitive Information Exposure**
- Hardcoded password variables
- Hardcoded API keys and credentials

#### 4. **Input Validation Issues**
- Unvalidated `input()` usage requiring sanitization

### 🎯 Use Cases
- ✅ Quick local security checks during development
- ✅ CI/CD pipeline integration for automated scanning
- ✅ Educational tool for learning secure coding practices
- ✅ Complement to enterprise SAST/DAST solutions
- ✅ Developer security awareness training

### 📚 What You'll Learn
- How SAST tools work at a fundamental level
- Common Python security anti-patterns
- Identifying and fixing code execution vulnerabilities
- Secure deserialization practices
- Protecting sensitive credentials in code
- Building security automation tools

### ⚠️ Important Notes
PyCodeScan is designed as an **educational and lightweight scanning tool** for developers. While effective for catching common insecure patterns, it should be complemented with:
- Comprehensive SAST tools (Bandit, SonarQube)
- DAST tools for runtime vulnerability detection
- Manual security code reviews
- Professional penetration testing services

---

**Last Updated:** July 2026  
**Portfolio Owner:** [@mactrevors349-afk](https://github.com/mactrevors349-afk)
