---
title: "Converting GIS data in FME Quick Translator"
layout: "home"
description: "FME (File Manipulation Engine) is a powerful software package that allows users to quickly convert spatial and non-spatial datasets into other formats to facilitate sharing and interoperability. One of its components, FME Quick Translator, is an easy-to-use utility that provides a straightforward translation workflow via a simple graphical user interface. This guide demonstrates how to use FME Universal Translator to convert geospatial data from one format to another using an older file format (ArcInfo Coverage, .e00) as an example."
staff:
    - name: Jordan Hale
created_date: 2016-04-26
permalink: "/"  #! Remove this if not the homepage
---

# Converting GIS data in FME Quick Translator

FME (File Manipulation Engine) is a powerful software package that allows users to quickly convert spatial and non-spatial datasets into other formats to facilitate sharing and interoperability. One of its components, FME Quick Translator, is an easy-to-use utility that provides a straightforward translation workflow via a simple graphical user interface. This guide demonstrates how to use FME Universal Translator to convert geospatial data from one format to another using an older file format (ArcInfo Coverage, .e00) as an example.

1. Launch FME Quick Translator from the Start Menu. On Map & Data Library computers, it is located in All Programs > FME Desktop 2012 SP4 > Utilities > FME Quick Translator.
2. Click on the Translate Data button on the far left of the toolbar to begin the translation process.  
![Screenshot of FME Quick Translator toolbar showing button to translate data.]({{ '/assets/images/1_translate-data.png' | relative_url }})

    Alternatively, browse to the location of the file in Windows, right-click on the name, and select Translate with FME Quick Translator.

    ![Screenshot of context menu in Windows Explorer showing option to translate data with FME Quick Translator.]({{ '/assets/images/2_translate-context-menu.png' | relative_url }})
3. In the Set Translation Parameters dialog, select the input dataset first by clicking on the … button next to the first Dataset box in the Reader section of the window. Browse to the location of the file and click Open to designate it as the file to be translated. The software should auto-detect the type of file and display it in the Format field directly above. If it does not auto-detect, you can use the dropdown menu to display a list of recently translated formats, or click on the … to select from a list. The Parameters… button provides options for advanced users specific to the input format.  
![Screenshots of Set Translation Parameters dialogue box in FME Quick Translator.]({{ '/assets/images/3_set-translation-parameter.png' | relative_url }})

    In the Writer section, select the data format that you would like to convert your dataset to by using the dropdown menu or the … button to select from the full list of translatable formats. Click on the … button next to the Dataset field to assign a location and filename to your output. Note that depending on the type of file you are translating to, you may not be assigning an output filename, but an output folder name – for example, because individual shapefiles are actually composed of several different component files, FME will prompt you to provide an output folder name, in which those files will be stored. Advanced options specific to the output format are again accessible by clicking on the Parameters… button. Click OK to begin the translation process.
4. The main console window will provide you with information regarding the progress of the translation process and alert you to any errors that may have occurred. At the end of the log, you will see a “Translation finished” message – at that point, your translated dataset is ready for use.  
![Screenshot showing translation log from FME Quick Translator.]({{ '/assets/images/4_translation-finished.png' | relative_url }})
5. *For advanced users*:  
You can use FME Quick Translator to batch convert multiple datasets of the same format. Copy them all to the same directory, then select the appropriate files by holding down the Ctrl key when selecting the dataset to translate. You can also use FME to transform your data from one coordinate system to another – click the … button next to the Coordinate System dropdown menu in the Writer section of the window to select from a list of geographic and projected coordinate systems.

 [converting-gis-data-using-fme-quick-translator.pdf](https://mdl.library.utoronto.ca/sites/default/public/converting-gis-data-using-fme-quick-translator.pdf)
 
 Discipline: [Architecture, Landscape & Design](https://mdl.library.utoronto.ca/discipline/architecture-landscape-design) | Technique: [Converting data formats](https://mdl.library.utoronto.ca/technique/converting-data-formats) | Tools: [FME](https://mdl.library.utoronto.ca/tools/fme-0) | Data Format: [Raster](https://mdl.library.utoronto.ca/data-format/raster), [Vector](https://mdl.library.utoronto.ca/data-format/vector)