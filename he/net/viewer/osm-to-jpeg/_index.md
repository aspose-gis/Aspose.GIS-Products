---
title: ממיר OSM ל-JPEG
url: /he/net/viewer/osm-to-jpeg/
weight: 10
layout: ""
---

## תיאור

ממיר קבצי OpenStreetMap (OSM) לתמונות JPEG. הכלי מאפשר המרת נתוני מיקום גיאוגרפי לפורמט תמונה, שימושי ליצירת מפות ויזואליות או להדגמת נתונים גיאוגרפיים.

## דרישות

*   Node.js
*   npm (node package manager)

## התקנה

1.  שכפל את המאגר:

    ```bash
    git clone [https://github.com/your-username/osm-to-jpeg](https://github.com/your-username/osm-to-jpeg)
    cd osm-to-jpeg
    ```
2.  התקן את התלויות:

    ```bash
    npm install
    ```

## שימוש

1.  הכנת קובץ OSM: ודא שברשותך קובץ OpenStreetMap בפורמט .osm או .pbf.
2.  הרצת הממיר: השתמש בפקודה הבאה כדי להמיר את קובץ ה-OSM ל-JPEG:

    ```bash
    node index.js -i input.osm -o output.jpeg
    ```

    *   `-i`: מציין את קובץ ה-OSM הקלט.
    *   `-o`: מציין את שם קובץ ה-JPEG הפלט.

## אפשרויות נוספות

*   `--width`: מגדיר את רוחב התמונה (ברירת מחדל: 800).
*   `--height`: מגדיר את גובה התמונה (ברירת מחדל: 600).
*   `--scale`: מגדיר את סקאלת הזום של המפה (ברירת מחדל: 1.0).

## דוגמאות

*   המרת קובץ OSM ל-JPEG עם רוחב של 1200 פיקסלים:

    ```bash
    node index.js -i input.osm -o output.jpeg --width 1200
    ```

*   המרת קובץ OSM ל-JPEG עם גובה של 800 פיקסלים וסקאלת זום של 0.5:

    ```bash
    node index.js -i input.osm -o output.jpeg --height 800 --scale 0.5
    ```

## הערות

*   הכלי משתמש בספריות חיצוניות לעיבוד נתוני OSM ויצירת תמונות. ודא שהספריות הללו מותקנות כראוי.
*   ניתן להתאים את פרמטרי המרה נוספים על ידי שינוי קוד המקור של הכלי.

---
