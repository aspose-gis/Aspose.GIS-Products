---
title: Python .NET Integration
linkTitle: Integracja z Pythonem .NET
weight: 10
description: Learn how to integrate Python with .NET applications.
url: /pl/python-net/
aliases:
  - python-dotnet
  - python-net-integration
---

## Introduction

This guide explains how to integrate Python into your .NET applications, enabling you to leverage the strengths of both languages.

## Prerequisites

*   **Python Installation:** Ensure that Python is installed on your system and accessible from the command line.
*   **.NET SDK:** You'll need the .NET SDK for development.
*   **IronPython (Optional):** For direct embedding, consider using IronPython. However, this approach has limitations.

## Methods of Integration

There are several ways to integrate Python with .NET:

1.  **IronPython:** This is a Python implementation written in C# that allows you to run Python code directly within your .NET application.
2.  **Command-Line Execution:** You can execute Python scripts from your .NET application using `Process` class.
3.  **Sockets/Inter-Process Communication (IPC):** Establish communication between a .NET process and a Python process via sockets or other IPC mechanisms.
4.  **Python for .NET Package:** This package provides a bridge to call Python code from C#

## IronPython Integration

### Setting up IronPython

1.  Install the `IronPython` NuGet package in your .NET project:

```csharp
// Example using Package Manager Console
Install-Package IronPython
```

2.  Reference the `IronPython.dll` and `Microsoft.Scripting.dll` assemblies.

### Basic Usage

```csharp
using IronPython.Hosting;
using Microsoft.Scripting.Hosting;

public class PythonIntegration
{
    public void RunPythonCode()
    {
        // Create a script engine
        var engine = Python.CreateEngine();

        // Define the scope
        var scope = engine.CreateScope();

        // Execute Python code
        string pythonScript = "print('Hello from Python!')";
        engine.Execute(pythonScript, scope);
    }
}
```

### Passing Data Between .NET and IronPython

You can pass data between .NET and IronPython using the `scope` object:

```csharp
using IronPython.Hosting;
using Microsoft.Scripting.Hosting;

public class PythonIntegration
{
    public void PassData()
    {
        var engine = Python.CreateEngine();
        var scope = engine.CreateScope();

        // Set a variable in the Python scope from .NET
        scope.SetVariable("name", "John Doe");

        // Execute Python code that uses the variable
        string pythonScript = "print('Hello, ' + name)";
        engine.Execute(pythonScript, scope);
    }
}
```

## Command-Line Execution

### Executing a Python Script

```csharp
using System;
using System.Diagnostics;

public class CommandLinePython
{
    public void ExecuteScript(string scriptPath)
    {
        Process process = new Process();
        process.StartInfo.FileName = "python";
        process.StartInfo.Arguments = scriptPath;
        process.StartInfo.RedirectStandardOutput = true;

        process.Start();
        string output = process.StandardOutput.ReadToEnd();
        process.WaitForExit();

        Console.WriteLine(output);
    }
}
```

## Sockets/IPC Integration

This approach involves creating a server in Python and a client in .NET to communicate over sockets or other IPC mechanisms. This allows for more complex interactions but requires more setup.

## Python for .NET Package

The `Python for .NET` package provides a convenient way to call Python code from C#. It simplifies the integration process by providing a bridge between the two languages.

### Installation

Install the `PythonNet` NuGet package:

```csharp
// Example using Package Manager Console
Install-Package PythonNet
```

### Usage

```csharp
using Python.Runtime;

public class PythonForDotNetIntegration
{
    public void CallPythonFunction()
    {
        // Initialize the Python runtime
        IronPython.Hosting.PythonEngine.Initialize();

        // Import a Python module
        using (Py.GIL())
        {
            dynamic myModule = Py.Import("my_module");

            // Call a function from the module
            var result = myModule.my_function(10, 20);

            Console.WriteLine($"Result: {result}");
        }
    }
}
```

## Considerations and Limitations

*   **Performance:**  Inter-process communication can introduce overhead.
*   **Debugging:** Debugging across language boundaries can be challenging.
*   **IronPython Compatibility:** IronPython may not support all Python libraries or features.
*   **Security:** Be cautious when executing external scripts, especially if they are user-provided.

## Conclusion

Integrating Python with .NET opens up a wide range of possibilities for combining the strengths of both languages. Choose the integration method that best suits your project's needs and complexity.
---
