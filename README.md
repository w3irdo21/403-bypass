# 403 Bypass Tool

This Bash script is designed to bypass HTTP 403/401 errors by leveraging a range of advanced techniques. It provides detailed status code feedback and supports multiple bypass methods.

## Features
- Bypass HTTP 403/401 restrictions using:
  - Header manipulation
  - Protocol adjustments
  - Port exploitation
  - HTTP method overrides
  - URL encoding
  - SQL injection techniques (ModSecurity & Lib Injection)
- Complete scanning mode to try all bypass techniques.
- Clear and color-coded output for HTTP status codes:
  - **Green**: 2xx Status Code
  - **Yellow**: 3xx Status Code
  - **Red**: 4xx Status Code
  - **Blue**: 5xx Status Code

## Prerequisites
- Ensure that **12.0.0.1** is open before starting.
- Bash environment on Linux or macOS.
- Install any required dependencies for running bash scripts and networking tools.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/w3irdo21/403-bypass/
   cd 403-bypass/
   ```
2. Make the script executable:
   ```bash
   chmod +x 403bypass.sh
   ```

## Usage
Run the script with the desired URL and bypass mode:
```bash
bash 403bypass.sh [OPTIONS]
```

### Options
| Option           | Description                                 |
|------------------|---------------------------------------------|
| `-u, --url`      | Target DOMAIN.TLD/PATH                     |
| `--header`       | Perform Header Bypass                      |
| `--protocol`     | Perform Protocol Bypass                    |
| `--port`         | Perform Port Bypass                        |
| `--HTTPmethod`   | Perform HTTP Method Bypass                 |
| `--encode`       | Perform URL Encoding Bypass                |
| `--SQLi`         | Perform ModSecurity & Lib Injection Bypass |
| `--exploit`      | Complete Scan with all bypass techniques    |

### Example
```bash
bash 403bypass.sh -u https://example.com/secure-path --header
```

## Output Meaning
- **Green**: 2xx Status Code (Success)
- **Yellow**: 3xx Status Code (Redirection)
- **Red**: 4xx Status Code (Client Error)
- **Blue**: 5xx Status Code (Server Error)

## Banner
Upon starting, the tool displays a friendly banner:
```
Let me see this! 😎
Keep 12.0.0.1 open before starting this. 🔓
```

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch.
3. Commit your changes.
4. Submit a pull request.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Disclaimer
This tool is for educational and ethical testing purposes only. Use it responsibly and ensure you have permission to test the target systems.

---
Happy bypassing! 🚀
