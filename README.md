# 🌐 CIDR Block IP Calculator

<p align="center">
  <img src="https://github.com/tcdoverlord/CIDR-Block-IP-Calculator/blob/main/cidrblockherovid.gif" alt="CIDR Block IP Calculator Demo" />
</p>

A lightweight, browser-based networking tool for calculating the total and displayed usable IPv4 addresses in a CIDR block.

Designed for subnet planning, networking education, subnetting practice, and cloud infrastructure learning.

---

<p align="left">
  <img src="https://img.shields.io/badge/HTML5-Frontend-orange" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-Styling-blue" alt="CSS3" />
  <img src="https://img.shields.io/badge/JavaScript-Logic-yellow" alt="JavaScript" />
  <img src="https://img.shields.io/badge/Networking-IPv4-green" alt="Networking IPv4" />
  <img src="https://img.shields.io/badge/Tool-CIDR%20Calculator-success" alt="CIDR Calculator" />
</p>

---

## 🎬 Demo

The GIF above shows the calculator being used in the browser.

No server or installation is required for basic use.

---

## 🚀 Features

- Calculate total IPv4 addresses for CIDR blocks
- Calculate the displayed reserved IP count
- Calculate the displayed usable IP count
- CIDR input validation
- Supports CIDR values from `/16` through `/28`
- Shows the calculation formula
- Shows a simple step-by-step math example
- Responsive interface for desktop and mobile
- Light and dark mode
- Reset calculator button
- Copy results to the clipboard
- Fully browser-based
- No frameworks
- No external libraries
- No build system required

---

## 🧮 How the Calculation Works

The calculator uses the standard IPv4 address-space formula:

```text
2^(32 - CIDR)
```

For example, for a `/16` CIDR block:

```text
2^(32 - 16)
= 2^16
= 65,536 total IP addresses
```

The calculator then subtracts 5 reserved IP addresses from the total:

```text
65,536 - 5
= 65,531 usable IP addresses
```

The same calculation is applied to the selected CIDR value from `/16` through `/28`.

> **Note:** The displayed usable-IP count in this project uses a fixed reservation of 5 addresses. It is intended as a simple planning/learning calculator rather than a complete subnetting implementation for every networking environment.

---

## 📖 How to Use

### Option 1 — Open Locally

1. Download or clone the repository.
2. Open:

```text
index.html
```

3. Enter a CIDR value such as:

```text
16
20
24
28
```

4. Click **Calculate**.
5. Review the total, reserved, usable, and formula results.

The calculator displays the `/` as part of the interface, so enter the number only.

### Option 2 — Git Clone

```bash
git clone https://github.com/tcdoverlord/CIDR-Block-IP-Calculator.git
cd CIDR-Block-IP-Calculator
```

Then open `index.html` in your browser.

---

## 📊 Example

### Input

```text
16
```

### Output

```text
Total IP addresses for /16: 65536
Reserved IPs: 5
Usable IPs: 65531
```

### Formula

```text
2^(32 - 16) = 65,536 total IPs
```

```text
65,536 - 5 = 65,531 usable IPs
```

---

## 🛠 Technologies

- HTML5
- CSS3
- JavaScript (ES6)

No frameworks or external dependencies are required.

---

## 📂 Project Structure

```text
CIDR-Block-IP-Calculator/
│
├── index.html
├── cidrblockherovid.gif
├── README.md
└── LICENSE
```

---

## 💡 Use Cases

- Network engineering learning
- IPv4 addressing education
- Subnetting practice
- IT training
- Cloud infrastructure planning
- AWS / Azure networking study
- Quick CIDR address calculations

---

## 🔒 Privacy

This calculator runs locally in the browser.

It does not require an account, server, database, or external service to perform calculations.

---

## 🤝 Contributing

Contributions are welcome.

You can improve the interface, add networking features, improve documentation, or submit bug fixes through GitHub issues and pull requests.

Before submitting changes, please test the calculator in a modern web browser.

---

## 👨‍💻 Author

**TCDOverLord**

GitHub:  
https://github.com/tcdoverlord

---

## 📄 License

See the [LICENSE](LICENSE) file for the license that applies to this project.
