---
title: Python .NET
url: /ko/python-net/
weight: 10
description: Learn how to use Python with .NET.
aliases:
  - python dotnet
---

## Introduction

This tutorial will show you how to use Python with .NET.

## Prerequisites

*   A machine with .NET installed
*   Python installed

## Installation

To install the IronPython package, you can use the following command:

```bash
pip install ironpython
```

## Basic Usage

Here's a simple example of how to use Python with .NET:

```csharp
using Microsoft.IronPython;

public class Example
{
    public static void Main(string[] args)
    {
        var engine = IronPython.Hosting.PythonEngine.Create();
        engine.Execute("print('Hello, world!')");
    }
}
```

## Advanced Usage

You can also use Python to write scripts that interact with .NET objects. For example, you can create a script that reads data from a database and displays it in a grid.

## Resources

*   [IronPython](https://ironpython.net/)
*   [Microsoft .NET](https://dotnet.microsoft.com/en-us/)

---
