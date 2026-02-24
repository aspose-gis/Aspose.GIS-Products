---
title: Python .NET
url: /uk/python-net/
weight: 10
layout: single
start: true
toc: true
draft: false
---

# Python .NET

## Overview

Python .NET is a set of libraries that allow you to use the Python language with the .NET runtime. This enables you to leverage the vast ecosystem of .NET libraries and tools while writing code in Python.

## Features

*   **Seamless Integration:** Integrate Python code into existing .NET applications.
*   **Access to .NET Libraries:** Utilize a wide range of .NET libraries from your Python code.
*   **Performance:** Benefit from the performance optimizations of the .NET runtime.
*   **Interoperability:** Easily call .NET functions and methods from Python, and vice versa.

## Installation

To install Python .NET, you can use the following command:

```bash
dotnet add package IronPython
```

## Basic Usage

Here's a simple example of how to use Python .NET:

```python
# This is a comment in Python
import clr
clr.AddReference("System")
from System import Console

Console.WriteLine("Hello from Python .NET!")
```

## Advanced Topics

*   **Creating Custom Assemblies:**  You can create custom .NET assemblies that are accessible from Python.
*   **Debugging:** Debug your Python .NET code using standard .NET debugging tools.
*   **Performance Tuning:** Optimize the performance of your Python .NET applications.

## Resources

*   [IronPython Documentation](https://ironpython.net/docs/)
*   [Python for .NET on GitHub](https://github.com/icsharpcode/IronPython)

## Conclusion

Python .NET provides a powerful way to combine the flexibility of Python with the performance and capabilities of the .NET platform.  It's an excellent choice for developers who want to leverage both worlds.
---
