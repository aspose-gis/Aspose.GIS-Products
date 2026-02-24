---
title: Python .NET
url: /ja/python-net/
weight: 10
---

# Python .NET

## Overview

Python for .NET allows you to host and run your Python code within a .NET environment. This enables you to leverage the power of both languages, combining Python's ease of use and extensive libraries with .NET's performance and rich ecosystem.

## Features

*   **IronPython:** A .NET implementation of Python.
*   **Integration:** Seamlessly integrate Python code into existing .NET applications.
*   **Performance:** Benefit from the optimized execution environment provided by .NET.
*   **Libraries:** Access a wide range of .NET libraries and frameworks from your Python code.

## Getting Started

### Prerequisites

*   .NET SDK
*   IronPython package

### Installation

```bash
# Install IronPython
Install-Package IronPython
```

### Basic Example

```python
# This is a simple Python script
print("Hello, .NET!")
```

This script can be executed within a .NET application using the `IronPython.Hosting` namespace.

## Advanced Usage

### Interoperability

Python for .NET provides excellent interoperability between Python and .NET code. You can easily call .NET methods from Python and vice versa.

### Debugging

Debugging Python code running in a .NET environment is straightforward, using standard .NET debugging tools.

## Resources

*   [IronPython Documentation](https://ironpython.net/)
*   [Python for .NET on GitHub](https://github.com/icsharpcode/IronPython)

---
