# EXgoldstandard
The gold standards are created for the evaluation and training of the EXCITE tools [EXmatcher](https://github.com/exciteproject/EXmatcher) and [EXparser](https://github.com/exciteproject/Exparser).

## GoldStandard for EXparser Step By Step:
1. Selecting Pdfs in German and English language.
    * To find more Information about our Selection method click [here](https://github.com/exciteproject/EXgoldstandard/tree/master/Goldstandard_EXparser)
2. Extracting Pdfs text In Layout format:
    * The used project to extracting layout from pdf is [Refex](https://github.com/exciteproject/refext)
3. Using EXRef-Identifier as a Reference String Identifier
    * EXRef-Identifier code is available [here](https://github.com/exciteproject/EXannotator/tree/master/EXRef-Identifier)
    * A live demo is available [here](http://excite.west.uni-koblenz.de/refanno/index.html)
    * A video tutorial to learn how to use this tool is available [here](https://www.youtube.com/watch?v=QSiqIHts23I&t=21s)
4. Again using [Refex](https://github.com/exciteproject/refext) to extract annotated references from layout files.
5. Using EXRef-Segmentation as a Meta Data Segmentation:
    * EXRef-Segmentation code is available [here](https://github.com/exciteproject/EXannotator/tree/master/EXRef-Segmentation)
    * A live demo is available [here](http://excite.west.uni-koblenz.de/seganno/index.html)
    * A video tutorial to learn how to use this tool is available [here](https://www.youtube.com/watch?v=xwed_XugR7E)
6. Using a python code to integrate the annotated meta data in layout file.
    * This code is available [here]()
7. Using generated Gold standard to train a model for [Exparser](https://github.com/exciteproject/Exparser)
    * To underestand how to train the EXparser please click [here](https://exparser.readthedocs.io/en/latest/)
