---
title: Python .NET
url: /th/python-net/
weight: 10
layout: single
start: true
toc: true
draft: false
---

![Python .NET Banner Image](images/python-dotnet-banner.png)

## Introduction

This guide provides an overview of using Python with the .NET framework. It covers setting up your environment, writing basic code, and exploring common use cases.

## Prerequisites

Before you begin, ensure you have the following installed:

*   **Python:** Download and install the latest version of Python from [python.org](https://www.python.org/).
*   **.NET SDK:** Install the .NET SDK from [microsoft.com](https://dotnet.microsoft.com/download).
*   **IronPython:** IronPython is an implementation of the Python programming language that runs on the .NET Framework. You can download it from [ironpython.net](http://ironpython.net/).

## Setting Up Your Environment

1.  **Install Required Packages:** Use pip to install the necessary packages:

    ```bash
    pip install ironpython
    ```

2.  **Verify Installation:** Check that IronPython is installed correctly by running:

    ```bash
    ironpython --version
    ```

## Basic Code Example

Here's a simple example of Python code using .NET:

```python
# This is a comment in Python
print("Hello from Python and .NET!")

# Accessing .NET functionality
from System import Console
Console.WriteLine("Hello from .NET!")
```

## Common Use Cases

*   **Scripting:** Automate tasks and workflows within the .NET environment.
*   **Extending .NET Applications:** Add Python scripting capabilities to existing .NET applications.
*   **Data Analysis:** Leverage Python's data science libraries with .NET infrastructure.
*   **Web Development:** Integrate Python web frameworks (like Django or Flask) with ASP.NET Core.

## Resources

*   [IronPython Documentation](http://ironpython.net/documentation/)
*   [Python.NET Documentation](https://github.com/pythonnet/pythonnet)
*   [Microsoft .NET Documentation](https://docs.microsoft.com/dotnet/)

---

