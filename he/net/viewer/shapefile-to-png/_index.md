---
title: המרת Shapefile ל-PNG
url: /he/net/viewer/shapefile-to-png/
weight: 10
layout: single
draft: false
description: מדריך להמרת קבצי Shapefile לתמונות PNG באמצעות צופה .NET.
---

## המרת Shapefile ל-PNG באמצעות צופה .NET

המדריך הזה מראה לך איך להמיר קבצי Shapefile לתמונות PNG באמצעות צופה .NET.

### דרישות

*   Visual Studio
*   .NET Framework 4.7.2 או גרסה מאוחרת יותר
*   צופה .NET

### שלבים

1.  צור פרויקט יישום קונסולה חדש ב-Visual Studio.
2.  הוסף הפניות לספריות ה-Viewer .NET.
3.  כתוב את הקוד הבא:

```csharp
// This is a comment in Hebrew: זהו תגובה בעברית
using NetMapViewer;
using System;
using System.IO;

namespace ShapefileToPng
{
    class Program
    {
        static void Main(string[] args)
        {
            // This is a comment in Hebrew: זהו תגובה בעברית
            string shapefilePath = "path/to/your/shapefile.shp";
            string pngFilePath = "path/to/your/output.png";

            try
            {
                using (var viewer = new MapViewer())
                {
                    viewer.LoadShapefile(shapefilePath);
                    viewer.SaveAsPng(pngFilePath);
                }

                Console.WriteLine($"Shapefile converted to PNG successfully: {pngFilePath}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting Shapefile to PNG: {ex.Message}");
            }
        }
    }
}
```

4.  החלף את `"path/to/your/shapefile.shp"` בנתיב לקובץ ה-Shapefile שלך.
5.  החלף את `"path/to/your/output.png"` בנתיב שבו אתה רוצה לשמור את תמונת ה-PNG שלך.
6.  הפעל את הפרויקט.

### הערות

*   ודא שהצופה .NET מותקן כראוי.
*   אם אתה מקבל שגיאות, בדוק את הנתיבים לקבצי Shapefile ו-PNG.
*   אתה יכול להתאים אישית את תמונת ה-PNG על ידי שינוי האפשרויות בשיטת `SaveAsPng`.

### פתרון בעיות

*   **לא ניתן למצוא את הקובץ:** ודא שהנתיב לקובץ Shapefile נכון.
*   **שגיאת פורמט לא נתמך:** ודא שקובץ ה-Shapefile הוא בפורמט תקין.
*   **שגיאה כללית:** בדוק את הודעת השגיאה כדי לקבל מידע נוסף על הבעיה.

### משאבים נוספים

*   [צופה .NET](https://example.com/net-viewer)
*   [Shapefile](https://en.wikipedia.org/wiki/Shapefile)
---
