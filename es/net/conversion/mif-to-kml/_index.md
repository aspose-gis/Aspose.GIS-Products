---
title: Convertir MIF a KML Datos GIS vía .NET 
weight: 50
url: /es/net/conversion/mif-to-kml/ 
description: Pruebe nuestras API On-Premise para la conversión de sus datos GIS en .NET Framework, .NET Core.
---

{{< blocks/products/pf/upper-banner h1="Convertir MIF a KML en C#" h2="Exportar MIF a KML usando API del lado del servidor, sin necesidad de softwares como ArcGIS, ArcMap, QGIS o Google Earth." logoImageSrc="https://www.aspose.cloud/templates/aspose/img/products/gis/aspose_gis-for-net.svg" sourceAdditionalConversionTag="" additionalConversionTag="KML" pfName="Aspose.GIS" subTitlepfName="para .NET" downloadUrl="" fileiconsmall1="PNG" fileiconsmall2="JPG" fileiconsmall3="BMP" fileiconsmall4="TIFF" fileiconsmall5="MIF" >}}

{{% blocks/products/pf/agp/content h2="Cómo convertir MIF a KML usando C#" %}}
 Para convertir MIF a KML, utilizaremos
 [Aspose.GIS for .NET](https://products.aspose.com/gis/net) 
 API que es una API GIS rica en funciones, potente y fácil de usar para la plataforma C#. Abra
 [NuGet](https://www.nuget.org/packages/aspose.gis) 
 administrador de paquetes, busque
 **Aspose.GIS** 
 e instale. También puede utilizar el siguiente comando desde la Consola del Administrador de Paquetes.

{{% blocks/products/pf/agp/code-block title="Comando" offSpacer="true" %}}
```cs
PM> Install-Package Aspose.GIS
```
{{% /blocks/products/pf/agp/code-block %}}
{{% /blocks/products/pf/agp/content %}}

{{< blocks/products/pf/agp/feature-section isGrey="true" >}}

{{% blocks/products/pf/agp/feature-section-col title="Pasos para convertir MIF a KML en C#" %}}
{{% blocks/products/pf/agp/text %}}
 La conversión se puede realizar con una sola línea de código al utilizar el
 *VectorLayer.Convert* 
 método. Toma 4 parámetros como se detalla a continuación.
{{% /blocks/products/pf/agp/text %}}

1.  Una ruta de archivo de tipo string al archivo MIF de origen  
2.  Controlador de origen para que la API sepa sobre el formato de entrada. Establézcalo en Drivers.MapInfoInterchange  
3.  La ruta de archivo de tipo string al archivo de datos KML de destino  
4.  Controlador de destino para especificar el formato de salida. Establézcalo en Drivers.Kml  
{{% /blocks/products/pf/agp/feature-section-col %}}

{{% blocks/products/pf/agp/feature-section-col title="Requisitos del sistema" %}}
{{% blocks/products/pf/agp/text %}}
 Nuestras API son compatibles con todas las plataformas y sistemas operativos principales. Antes de ejecutar el código a continuación, asegúrese de tener los siguientes requisitos previos en su sistema.
{{% /blocks/products/pf/agp/text %}}
{{% /blocks/products/pf/agp/feature-section-col %}}

{{% blocks/products/pf/agp/code-block title="Guardar MIF como KML - C#" offSpacer="" %}}
```cs
// Convertir datos GIS de MIF a datos de KML
VectorLayer.Convert(dir + "example.mif", Drivers.MapInfoInterchange, dir + "output.kml", Drivers.Kml);
```
{{% /blocks/products/pf/agp/code-block %}}

{{< /blocks/products/pf/agp/feature-section >}}

{{< blocks/products/pf/agp/demobox sectionTitle="MIF a KML Demostraciones en vivo" sectionDescription="Convierta MIF a KML ahora mismo visitando nuestro [sitio web de demostraciones en vivo](https://products.aspose.app/gis/conversion/mif-to-kml). La demostración en vivo tiene los siguientes beneficios" >}}
    {{< blocks/products/pf/agp/democard icon="fa-cogs" text=" No es necesario descargar la API de Aspose GIS." >}}
    {{< blocks/products/pf/agp/democard icon="fa-edit" text=" Simplemente seleccione KML como formato de salida y." >}}
    {{< blocks/products/pf/agp/democard icon="fa-file-text" text=" Suba su archivo MIF, se convertirá instantáneamente a KML." >}}
    {{< blocks/products/pf/agp/democard icon="fa-download" text=" Obtendrá el enlace de descarga." >}}

    {{% blocks/products/pf/agp/content h2="Biblioteca GIS .NET" %}}
     Aspose.GIS para .NET es una API de manipulación y conversión de datos GIS. Admite completamente la lectura, escritura y conversión de formatos de datos GIS famosos como Shapefiles ESRI, GeoJSON, TopoJSON, Base de datos Geográfica ESRI, Lenguaje de Marcado de Geografía, Google Earth, Formato de Intercambio GPS, Formatos MapInfo y OpenStreetMap. Es una API independiente basada en .NET y no requiere ningún software basado en GIS como ArcGIS / ArcMap, QGIS, etc. 
    {{% /blocks/products/pf/agp/content %}}

    {{< blocks/products/pf/agp/about-file-section >}}
        {{< blocks/products/pf/agp/about-file-text fileFormat="MIF" readMoreLink="https://docs.fileformat.com/gis/kml/" >}}
{{mif}}
Leer más
        {{< /blocks/products/pf/agp/about-file-text >}}

        {{< blocks/products/pf/agp/about-file-text fileFormat="KML" readMoreLink="" >}}
KML, (Lenguaje de Marcado Clave) contiene información geoespacial en notación XML. Los archivos guardados como KML se pueden abrir en aplicaciones de Sistemas de Información Geográfica (GIS) siempre que lo admitan. Muchas aplicaciones han comenzado a proporcionar soporte para el formato de archivo KML después de que se adoptó como estándar internacional. KML utiliza una estructura basada en etiquetas con elementos y atributos anidados. Todas las etiquetas distinguen entre mayúsculas y minúsculas y, según la Referencia KML, es importante seguir el orden de estas etiquetas.
Leer más
        {{< /blocks/products/pf/agp/about-file-text >}}
    {{< /blocks/products/pf/agp/about-file-section >}}
{{< /blocks/products/pf/agp/demobox >}}

{{< blocks/products/pf/agp/other-supported-section title="Otras conversiones admitidas" subTitle="También puede convertir MIF a muchos otros formatos de archivo, incluidos algunos enumerados a continuación." >}}
    {{< blocks/products/pf/agp/other-supported-section-item href="https://products.aspose.com/gis/net/conversion/mif-to-geojson" name="MIF A GEOJSON" description="Formato basado en JSON" >}}
    {{< blocks/products/pf/agp/other-supported-section-item href="https://products.aspose.com/gis/net/conversion/mif-to-shx" name="MIF A SHX" description="Extensión de archivo Shapefile" >}}
{{< /blocks/products/pf/agp/other-supported-section >}}
