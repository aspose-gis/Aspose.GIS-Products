---
title: Преобразование Shapefile в PNG
url: /ru/net/viewer/shapefile-to-png/
weight: 10
layout: single
draft: false
description: Инструкции по преобразованию файлов shapefile в изображения PNG с помощью .NET Viewer.
---

## Преобразование Shapefile в PNG с использованием .NET Viewer

Этот документ содержит инструкции по преобразованию файлов shapefile в изображения PNG с использованием .NET Viewer.

### Необходимые условия

Прежде чем начать, убедитесь, что у вас есть следующее:

*   Установленный .NET SDK
*   Visual Studio или другая среда разработки C#
*   Библиотека .NET Viewer

### Шаги

1.  **Создайте новый проект C#:** Создайте новый консольный проект C# в Visual Studio или другой среде разработки.
2.  **Добавьте ссылку на библиотеку .NET Viewer:** Добавьте ссылку на библиотеку .NET Viewer в свой проект.
3.  **Импортируйте необходимые пространства имен:** Импортируйте пространства имен `NetMapViewer` и `NetMapViewer.Shapes`.

```csharp
using NetMapViewer;
using NetMapViewer.Shapes;
```

4.  **Создайте экземпляр класса `ShapefileToPngConverter`:** Создайте экземпляр класса `ShapefileToPngConverter`, передав путь к файлу shapefile в качестве аргумента конструктора.

```csharp
string shapefilePath = "path/to/your/shapefile.shp";
ShapefileToPngConverter converter = new ShapefileToPngConverter(shapefilePath);
```

5.  **Укажите параметры преобразования:** Установите необходимые параметры преобразования, такие как ширина и высота изображения, цветовая схема и т.д.

```csharp
converter.Width = 800;
converter.Height = 600;
converter.ColorSchema = ColorSchema.BlueDarkGreen;
```

6.  **Выполните преобразование:** Вызовите метод `Convert()` для выполнения преобразования shapefile в PNG изображение. Укажите путь к файлу, в который будет сохранено изображение.

```csharp
string pngFilePath = "path/to/your/output.png";
converter.Convert(pngFilePath);
```

### Пример кода

```csharp
using NetMapViewer;
using NetMapViewer.Shapes;
using System;
using System.IO;

namespace ShapefileToPngConverter
{
    class Program
    {
        static void Main(string[] args)
        {
            // Укажите путь к файлу shapefile
            string shapefilePath = "path/to/your/shapefile.shp";

            // Укажите путь к выходному PNG файлу
            string pngFilePath = "path/to/your/output.png";

            try
            {
                // Создайте экземпляр класса ShapefileToPngConverter
                ShapefileToPngConverter converter = new ShapefileToPngConverter(shapefilePath);

                // Установите параметры преобразования (необязательно)
                converter.Width = 800;
                converter.Height = 600;
                converter.ColorSchema = ColorSchema.BlueDarkGreen;

                // Выполните преобразование
                converter.Convert(pngFilePath);

                Console.WriteLine($"Shapefile успешно преобразован в PNG: {pngFilePath}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Произошла ошибка при преобразовании shapefile: {ex.Message}");
            }
        }
    }
}
```

### Дополнительные параметры

Класс `ShapefileToPngConverter` предоставляет следующие дополнительные параметры:

*   `Width`: Ширина выходного изображения в пикселях.
*   `Height`: Высота выходного изображения в пикселях.
*   `ColorSchema`: Цветовая схема для отображения данных shapefile.
*   `ZoomLevel`: Уровень масштабирования для отображения данных shapefile.
*   `RotationAngle`: Угол поворота для отображения данных shapefile.

### Решение проблем

Если у вас возникли проблемы при преобразовании shapefile в PNG изображение, попробуйте следующее:

*   Убедитесь, что файл shapefile существует и доступен для чтения.
*   Убедитесь, что у вас есть права на запись в указанный выходной каталог.
*   Проверьте параметры преобразования и убедитесь, что они соответствуют вашим требованиям.
*   Обратитесь к документации .NET Viewer или обратитесь за помощью к сообществу разработчиков.

### Заключение

В этом документе описаны шаги по преобразованию файлов shapefile в изображения PNG с использованием .NET Viewer. Следуя этим инструкциям, вы сможете легко преобразовывать свои файлы shapefile в удобный для просмотра формат изображений.
---
