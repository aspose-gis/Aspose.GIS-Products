---
title: Python .NET Integration
linkTitle: Python .NET Entegrasyonu
weight: 10
url: /tr/python-net/
description: Learn how to integrate Python with .NET applications.
açıklama: Python'u .NET uygulamalarıyla nasıl entegre edeceğinizi öğrenin.
---

## Introduction
## Giriş

This guide explains how to use Python within a .NET application.
Bu kılavuz, Python'un bir .NET uygulaması içinde nasıl kullanılacağını açıklar.  You can embed Python interpreters, execute Python scripts, and leverage Python libraries directly from your C# code.
Python yorumlayıcılarını gömme, Python komut dosyalarını çalıştırma ve Python kitaplıklarından doğrudan C# kodunuzdan yararlanma konularını ele alabilirsiniz.

## Prerequisites
## Ön Koşullar

*   **IronPython:**  A .NET implementation of Python. You'll need to install this separately.
    *   **IronPython:** Python'un bir .NET uygulamasıdır. Ayrı olarak yüklemeniz gerekecektir.
*   **.NET SDK:** Make sure you have the latest .NET SDK installed.
    *   **.NET SDK:** En son .NET SDK'sının yüklü olduğundan emin olun.
*   **Basic Python Knowledge:** Familiarity with Python syntax and common libraries is helpful.
    *   **Temel Python Bilgisi:** Python sözdizimi ve yaygın kitaplıklar hakkında bilgi faydalıdır.

## Installation
## Kurulum

1.  **Install IronPython:** Download the appropriate version of IronPython for your .NET framework from [IronPython website](https://ironpython.net/).
    *   **IronPython'u Yükleyin:** .NET çerçeveniz için uygun IronPython sürümünü [IronPython web sitesinden](https://ironpython.net/) indirin.
2.  **Create a New .NET Project:** Use Visual Studio or your preferred IDE to create a new console application project.
    *   **Yeni Bir .NET Projesi Oluşturun:** Yeni bir konsol uygulaması projesi oluşturmak için Visual Studio veya tercih ettiğiniz geliştirme ortamını kullanın.
3.  **Add IronPython Reference:** In your project, add a reference to the `IronPython` assembly.
    *   **IronPython Referansını Ekleyin:** Projenizde `IronPython` derlemesine bir referans ekleyin.

## Basic Usage
## Temel Kullanım

Here's a simple example of how to execute a Python script from your C# code:
İşte C# kodunuzdan bir Python komut dosyasını çalıştırmanın basit bir örneği:

```csharp
// Example C# Code
using IronPython.Hosting;
using Microsoft.Scripting.Hosting;

public class Program
{
    public static void Main(string[] args)
    {
        ScriptEngine engine = Python.CreateEngine();
        IConsoleOutputWriter consoleOut = new ConsoleOutputWriter(Console.Out);
        engine.OutputOption = consoleOut;

        // Execute a simple Python script
        string pythonScript = @"
print('Hello from Python!')
";

        ScriptScope scope = engine.CreateScope();
        dynamic result = engine.Execute(pythonScript, scope);
    }
}
```

This code snippet creates an IronPython engine, sets up output redirection, and then executes a simple Python script that prints "Hello from Python!".
Bu kod parçacığı bir IronPython motoru oluşturur, çıktı yönlendirmesini ayarlar ve ardından "Python'dan merhaba!" yazdıran basit bir Python komut dosyası çalıştırır.

## Advanced Integration
## Gelişmiş Entegrasyon

*   **Passing Data:** You can pass data between C# and Python using script scope objects.
    *   **Veri Aktarımı:** Verileri C# ve Python arasında betik kapsamı nesnelerini kullanarak aktarabilirsiniz.
*   **Calling Python Functions:**  You can expose Python functions to your C# code and call them directly.
    *   **Python Fonksiyonlarını Çağırma:** Python fonksiyonlarınızı C# kodunuza açabilir ve doğrudan bunları çağırabilirsiniz.
*   **Using Python Libraries:** Import and use Python libraries within your .NET application.
    *   **Python Kitaplıklarını Kullanma:** Python kitaplıklarını .NET uygulamanızda içe aktarın ve kullanın.

## Error Handling
## Hata Yönetimi

When working with IronPython, it's important to handle potential errors gracefully.  Use `try-catch` blocks to catch exceptions that may be thrown by the Python interpreter.
IronPython ile çalışırken, olası hataları zarif bir şekilde ele almak önemlidir. Python yorumlayıcısı tarafından atılabilecek istisnaları yakalamak için `try-catch` bloklarını kullanın.

## Resources
## Kaynaklar

*   **IronPython Documentation:** [https://ironpython.net/](https://ironpython.net/)
    *   **IronPython Belgeleri:** [https://ironpython.net/](https://ironpython.net/)
*   **Microsoft Scripting Engine:** [https://www.microsoft.com/en-us/scripting/develop/ironpython/](https://www.microsoft.com/en-us/scripting/develop/ironpython/)
    *   **Microsoft Betik Motoru:** [https://www.microsoft.com/en-us/scripting/develop/ironpython/](https://www.microsoft.com/en-us/scripting/develop/ironpython/)

---
