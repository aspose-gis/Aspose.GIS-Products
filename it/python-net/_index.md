---
title: Python .NET
url: /it/python-net/
weight: 10
layout: single
start: true
toc: false
draft: false

---

## Introduzione

Questo documento fornisce una panoramica di come utilizzare Python con .NET.

## Prerequisiti

*   .NET SDK installato
*   Python installato

## Installazione

Per utilizzare Python con .NET, è necessario installare il pacchetto `pythonnet`. Questo può essere fatto utilizzando NuGet:

```bash
Install-Package pythonnet
```

## Esempio

Ecco un semplice esempio di come utilizzare Python con .NET:

```csharp
using IronPython.Hosting;
using Microsoft.Scripting.Hosting;

public class Example
{
    public static void Main(string[] args)
    {
        // Crea un engine Python
        var engine = Python.CreateEngine();

        // Crea una scope Python
        var scope = engine.CreateScope();

        // Esegui codice Python
        scope.Execute("print('Ciao dal mondo di Python!')");
    }
}
```

Questo esempio crea un engine Python, crea una scope Python ed esegue il codice Python `print('Ciao dal mondo di Python!')`. Questo stamperà "Ciao dal mondo di Python!" sulla console.

## Considerazioni aggiuntive

*   Assicurati che la versione di Python sia compatibile con la versione di .NET che stai utilizzando.
*   Il pacchetto `pythonnet` richiede Visual C++ Redistributable per funzionare. Assicurati che questo sia installato sul tuo sistema.
*   Quando si lavora con librerie Python, potrebbe essere necessario installarle usando `pip`.

## Risoluzione dei problemi

Se riscontri problemi durante l'utilizzo di Python con .NET, consulta la documentazione del pacchetto `pythonnet` per ulteriori informazioni sulla risoluzione dei problemi.
---
