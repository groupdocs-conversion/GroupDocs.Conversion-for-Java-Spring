![Convert pdf to doc or doc to pdf](https://raw.githubusercontent.com/groupdocs-conversion/groupdocs-conversion.github.io/master/resources/image/banner.png "GroupDocs.Conversion")
# GroupDocs.Conversion for Java Spring Example
GroupDocs.Conversion for Java Spring UI Example
###### version 0.0.0

[![Build Status](https://travis-ci.org/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Spring.svg?branch=master)](https://travis-ci.org/groupdocs-conversion/GroupDocs.Conversion-for-Java-Spring)
[![Maintainability](https://api.codeclimate.com/v1/badges/6db148bfbdc7912b07e6/maintainability)](https://codeclimate.com/github/groupdocs-conversion/GroupDocs.Conversion-for-Java-Spring/maintainability)
[![GitHub license](https://img.shields.io/github/license/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Spring.svg)](https://github.com/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Spring/blob/master/LICENSE)

## System Requirements
- Java 8 (JDK 1.8)
- Maven 3


## Document converter with Java API

**GroupDocs.Conversion for Java API** is a library that allows you to **convert word to PDF, PNG, JPG** and to many other document or image formats supported by the library. Using powerful and flexible GroupDocs.Conversion API you will be able to convert multitude document formats with a wide set of different options.

This web application allows you to convert documents between different formats using simple modern UI. While it can be used as a standalone application it also can be integrated as part of your project.

**Note:** without a license application will run in trial mode, purchase [GroupDocs.Conversion for Java license](https://purchase.groupdocs.com/order-online-step-1-of-8.aspx) or request [GroupDocs.Conversion for Java temporary license](https://purchase.groupdocs.com/temporary-license).

| Document family        | Supported formats                                                         | Supported conversions                                                                                                                                |
| ------------------------ | ------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| Microsoft Word           | `Doc`,`Docm`,`Docx`,`Dot`,`Dotm`,`Dotx`,`Rtf`,`Txt`,`Odt`,`Ott`           | `Word to Rtf`,`Word to Txt`,`Word to Html`,`Word to Odt`,`Word to Ott`,`Word to Epub`,`Word to Pdf`,`Word to Image`,`Word to Cells`,`Word to Slides` |
| Microsoft Excel          | `Xls`,`Xls2003`,`Xlsb`,`Xlsm`,`Xlsx`                                      | `Excel to Word`,`Excel to Pdf`,`Excel to Epub`,`Excel to Html`,`Excel to Image`,`Excel to Slides`                                                    |
| Portable Document Format | `Pdf`                                                                     | `Pdf to Word`,`Pdf to Epub`,`Pdf to Html`,`Pdf to Image`,`Pdf to Cells`,`Pdf to Slides`                                                              |
| Microsoft PowerPoint     | `Ppt`,`Pps`,`Pptx`,`Ppsx`,`Odp`                                           | `Slides to Word`,`Slides to Pdf`,`Slides to Epub`,`Slides to Html`,`Slides to Image`,`Slides to Excel`                                               |
| Microsoft Visio          | `Vsd`,`Vsdx`,`Vss`,`Vst`,`Vsx`,`Vtx`,`Vdw`,`Vdx`,`Svg`                    | `Visio to Word`,`Visio to Pdf`,`Visio to Epub`,`Visio to Html`,`Visio to Image`,`Visio to Excel`,`Visio to Slides`                                   |
| Microsoft Project        | `Mpt`,`Mpp`                                                               | `Tasks to Word`,`Tasks to Pdf`,`Tasks to Epub`,`Tasks to Html`,`Tasks to Image`,`Tasks to Excel`,`Tasks to Slides`                                   |
| HTML                     | `Html`                                                                    | `Html to Word`,`Html to Pdf`,`Html to Epub`,`Html to Cells`,`Html to Slides`                                                                         |
| Images                   | `Xps`,`Tiff`,`Tif`,`Jpeg`,`Jpg`,`Png`,`Gif`,`Bmp`,`Ico`,`Dxf`,`Dwg`,`Psd` | `Image to Word`,`Image to Pdf`,`Image to Epub`,`Image to Html`,`Image to Image`,`Image to Cells`,`Image to Slides`                                   | 

## Demo Video
Coming soon


## Features

- Clean, modern and intuitive design
- Easily switchable colour theme (create your own colour theme in 5 minutes)
- Responsive design
- Convert individual documents
- Batch convert multiple files
- Mobile support (open application on any mobile device)
- HTML and image modes
- Drag and Drop support
- Upload documents
- Cross-browser support (Safari, Chrome, Opera, Firefox)
- Cross-platform support (Windows, Linux, MacOS)


## How to run

You can run this sample by one of following methods


#### Build from source

Download [source code](https://github.com/groupdocs-conversion/GroupDocs.Conversion-for-Java-Spring/archive/master.zip) from github or clone this repository.

```bash
git clone https://github.com/groupdocs-conversion/GroupDocs.Conversion-for-Java-Spring
cd GroupDocs.Conversion-for-Java-Spring
mvn clean spring-boot:run
## Open http://localhost:8080/conversion/ in your favorite browser.
```

#### Build war from source

Download [source code](https://github.com/groupdocs-conversion/GroupDocs.Conversion-for-Java-Spring/archive/master.zip) from github or clone this repository.

```bash
git clone https://github.com/groupdocs-conversion/GroupDocs.Conversion-for-Java-Spring
cd GroupDocs.Conversion-for-Java-Spring
mvn package -P war
## Deploy this war on any server
```

#### Binary release (with all dependencies)

Download [latest release](https://github.com/groupdocs-conversion/GroupDocs.Conversion-for-Java-Spring/releases/latest) from [releases page](https://github.com/groupdocs-conversion/GroupDocs.Conversion-for-Java-Spring/releases). 

**Note**: This method is **recommended** for running this sample behind firewall.

```bash
curl -J -L -o release.tar.gz https://github.com/groupdocs-conversion/GroupDocs.Conversion-for-Java-Spring/releases/download/0.0.0/release.tar.gz
tar -xvzf release.tar.gz
cd release
java -jar conversion-spring-0.0.0.jar configuration.yaml
## Open http://localhost:8080/Conversion/ in your favorite browser.
```

#### Docker image
Use [docker](https://hub.docker.com/u/groupdocs) image.

```bash
mkdir DocumentSamples
mkdir Licenses
docker run -p 8080:8080 --env application.hostAddress=localhost -v `pwd`/DocumentSamples:/home/groupdocs/app/DocumentSamples -v `pwd`/Licenses:/home/groupdocs/app/Licenses groupdocs/conversion
## Open http://localhost:8080/Conversion/ in your favorite browser.
```

## Configuration
For all methods above you can adjust settings in `configuration.yml`. By default in this sample will lookup for license file in `./Licenses` folder, so you can simply put your license file in that folder or specify relative/absolute path by setting `licensePath` value in `configuration.yml`. 

### Conversion configuration options

| Option                             | Type    |   Default value   | Description                                                                                                                                  |
| ---------------------------------- | ------- |:-----------------:|:-------------------------------------------------------------------------------------------------------------------------------------------- |
| **`filesDirectory`**               | String  | `DocumentSamples` | Files directory path. Indicates where uploaded and predefined files are stored. It can be absolute or relative path                          |
| **`resultDirectory`**              | String  |                   | Absolute path to result files directory                                                                                                      |

## License
The MIT License (MIT). 

Please have a look at the LICENSE.md for more details

## GroupDocs Conversion on other platforms & frameworks

- [Document converter](https://github.com/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Dropwizard) with JAVA Dropwizard 
- [Document converter](https://github.com/groupdocs-Conversion/GroupDocs.Conversion-for-.NET-MVC) with .NET MVC 
- [Document converter](https://github.com/groupdocs-Conversion/GroupDocs.Conversion-for-.NET-WebForms) with .NET WebForms 


## Resources
- **Website:** [www.groupdocs.com](http://www.groupdocs.com)
- **Product Home:** [GroupDocs.Conversion for Java](https://products.groupdocs.com/conversion/java)
- **Product API References:** [GroupDocs.Conversion for Java API](https://apireference.groupdocs.com)
- **Download:** [Download GroupDocs.Conversion for Java](http://downloads.groupdocs.com/conversion/java)
- **Documentation:** [GroupDocs.Conversion for Java Documentation](https://docs.groupdocs.com/dashboard.action)
- **Free Support Forum:** [GroupDocs.Conversion for Java Free Support Forum](https://forum.groupdocs.com/c/conversion)
- **Paid Support Helpdesk:** [GroupDocs.Conversion for Java Paid Support Helpdesk](https://helpdesk.groupdocs.com)
- **Blog:** [GroupDocs.Conversion for Java Blog](https://blog.groupdocs.com/category/groupdocs-conversion-product-family)