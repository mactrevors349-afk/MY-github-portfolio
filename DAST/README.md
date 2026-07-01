# 🔍 Dynamic Application Security Testing (DAST) Projects

Welcome to the DAST section of my portfolio. This folder contains projects focused on **Dynamic Application Security Testing**, runtime vulnerability detection, and web application security analysis.

---

## 🛡️ WebInsight Scout - DAST Vulnerability Scanner

**Repository:** [DAST-tool-PyCodeScan](https://github.com/mactrevors349-afk/DAST-tool-PyCodeScan)

### 📋 Project Overview

A basic Python **Dynamic Application Security Testing (DAST)** tool for educational use as well as detecting insecure patterns and vulnerabilities in external links (URLs). WebInsight Scout is an educational tool that demonstrates how DAST tools operate at a conceptual level. It performs passive security analysis on web applications without injecting malicious payloads.

### 🔑 Key Features

- 🔍 **Basic Web Interaction**: Uses the `requests` library to make HTTP requests and checks HTTP status codes and response headers
- 📄 **HTML Content Parsing**: Employs BeautifulSoup to parse HTML responses for link/form discovery and HTML comment analysis
- 🔎 **Keyword-Based Vulnerability Detection**: Analyzes response body for security indicators (error messages, stack traces, database keywords, etc.)
- 🛡️ **Robust Error Handling**: Connection timeouts with configurable timeout periods and graceful degradation on failures
- 📊 **Simplified Reporting**: Collects findings with type, severity, and description, grouped by severity levels (High, Medium, Low)
- ⚡ **Educational & Practical**: Built for developers learning security best practices and DAST methodology fundamentals

### 🛠️ Technologies Used

- **Language:** Python
- **Libraries:** `requests`, `beautifulsoup4`
- **Core Concepts:** HTTP protocol, HTML parsing, Pattern-based vulnerability detection
- **Focus Areas:** DAST, Runtime vulnerability detection, Security scanning automation

### 📂 Project Architecture

```
DAST-tool-PyCodeScan/
├── DAST_VULNERABILITY_SCANNER.py    # Main scanner implementation
├── README.md                         # Full documentation
├── requirements.txt                  # Python dependencies
└── PORTFOLIO_ENTRY.md               # Portfolio documentation
```

### 🚀 Getting Started

To use WebInsight Scout:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/mactrevors349-afk/DAST-tool-PyCodeScan.git
   cd DAST-tool-PyCodeScan
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run a vulnerability scan:**
   ```bash
   python DAST_VULNERABILITY_SCANNER.py https://example.com
   ```

4. **Review findings:**
   - View findings grouped by severity (High, Medium, Low)
   - Understand identified security indicators
   - Learn DAST concepts at a practical level

### 🔗 Live Links

- **GitHub Repository:** [mactrevors349-afk/DAST-tool-PyCodeScan](https://github.com/mactrevors349-afk/DAST-tool-PyCodeScan)
- **View Code:** [Full repository on GitHub](https://github.com/mactrevors349-afk/DAST-tool-PyCodeScan/tree/main)

### 📊 Detection Capabilities

#### HTML Analysis
- **Link Discovery**: Identifies all hyperlinks and flags suspicious attributes (`javascript:`, `data:`)
- **Form Detection**: Finds forms and flags insecure patterns (e.g., password fields with GET method)
- **Comment Analysis**: Scans HTML comments for sensitive keywords (`password`, `api_key`, `secret`, `admin`, `token`)

#### Response Body Analysis
- **Information Disclosure**: Detects error messages and exception details that leak system information
- **Database References**: Flags keywords indicating database operations
- **JavaScript Errors**: Identifies client-side vulnerabilities

### 🎯 Use Cases

- ✅ Educational tool for learning DAST principles
- ✅ Quick security checks for passive vulnerability detection
- ✅ Developer security awareness training
- ✅ Complement to passive security scanning workflows
- ✅ Learning HTTP protocol and web application security concepts

### 📚 What You'll Learn

- Basic HTTP protocol concepts and request/response handling
- HTML parsing and analysis fundamentals
- Pattern matching for security indicator detection
- Error handling and resilient code practices
- DAST methodology at a conceptual level
- Limitations of passive security scanning

### ⚠️ Important Limitations

This is an **educational and conceptual tool only**, with significant limitations:

- ❌ **No Payload Injection**: Does NOT actively test for vulnerabilities through payload injection
- ❌ **No Web Crawling**: Processes single URLs without autonomous path discovery
- ❌ **Simple Pattern Matching**: High potential for false positives and false negatives
- ❌ **Passive Analysis Only**: Cannot detect injection vulnerabilities (SQL, XSS, Command Injection)
- ❌ **No Session Management**: Lacks authentication handling and stateful testing
- ❌ **No Contextual Analysis**: Cannot understand application business logic or data flow

### 🎓 Educational Value

Perfect for learning:
- ✓ HTTP protocol fundamentals
- ✓ HTML parsing with BeautifulSoup
- ✓ Web security basics and vulnerability types
- ✓ Limitations of passive security scanning
- ✓ How real DAST tools work at a conceptual level

---

**Last Updated:** July 2026  
**Portfolio Owner:** [@mactrevors349-afk](https://github.com/mactrevors349-afk)
