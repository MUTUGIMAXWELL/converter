# NumConvert Pro - Project Documentation

## Overview
NumConvert Pro is a Progressive Web App (PWA) that provides real-time conversion between different number systems including binary, decimal, hexadecimal, and octal. It features a modern dark-themed interface with instant results and one-click copy functionality.

![NumConvert Pro](https://img.shields.io/badge/Version-1.0-blue) ![PWA](https://img.shields.io/badge/PWA-Enabled-green) ![License](https://img.shields.io/badge/License-MIT-lightgrey)

## 🚀 Features

### Core Functionality
- **⚡ Real-time Conversion** - Instant results as you type
- **🔮 Auto-detection** - Automatically detects number system based on input patterns
- **📋 One-Click Copy** - Copy any result with a single click
- **🔄 Multi-system Support** - Convert between four number systems simultaneously

### Supported Number Systems
| System | Base | Prefix | Example Input |
|--------|------|--------|---------------|
| Binary | 2 | `0b` | `1010`, `0b1010` |
| Decimal | 10 | - | `255`, `42` |
| Hexadecimal | 16 | `0x` | `FF`, `0xFF` |
| Octal | 8 | `0o` | `377`, `0o377` |

### PWA Capabilities
- 📱 **Installable** - Can be installed as a native app
- 🔌 **Offline Support** - Works without internet connection
- 🎯 **App-like Experience** - Standalone display mode

## 🛠️ Project Structure

## 🎨 UI Components

### Main Interface
- **Converter Card** - Input field and system selector
- **Result Cards** - Individual cards for each number system
- **Feature Cards** - Highlighting app capabilities
- **Install Button** - Fixed position for PWA installation

### Color Scheme
```css
--primary: #6366f1;
--primary-dark: #4f46e5;
--secondary: #10b981;
--dark-bg: #0f172a;
--card-bg: #1e293b;
--text: #f8fafc;
const patterns = {
    binary: /^[01]+$|^0b[01]+$/i,
    hexadecimal: /^[0-9a-f]+$|^0x[0-9a-f]+$/i,
    octal: /^[0-7]+$|^0o[0-7]+$/i,
    decimal: /^\d+$/
};
{
  "name": "Number System Converter",
  "short_name": "NumConverter",
  "description": "Convert numbers between binary, decimal, hexadecimal, and octal systems",
  "start_url": "./",
  "display": "standalone"
}
graph LR
    A[User Input] --> B[Input Cleaning]
    B --> C[System Detection]
    C --> D[Decimal Conversion]
    D --> E[Target Conversion]
    E --> F[Display Results]
