# GroupDocs.Conversion for Java Spring Example
GroupDocs.Conversion for Java Spring UI Example
###### version 0.0.1

[![Build Status](https://travis-ci.org/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Spring.svg?branch=master)](https://travis-ci.org/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Spring)
[![Maintainability](https://api.codeclimate.com/v1/badges/6db148bfbdc7912b07e6/maintainability)](https://codeclimate.com/github/groupdocs-conversion/GroupDocs.Conversion-for-Java-Spring/maintainability)
[![GitHub license](https://img.shields.io/github/license/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Spring.svg)](https://github.com/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Spring/blob/master/LICENSE)

## System Requirements
- Java 8 (JDK 1.8)
- Maven 3


## Document converter with Java API

**GroupDocs.Conversion for Java API** is a library that allows you to **convert word to PDF, PNG, JPG** or any other document or image format. Using powerful and flexible API GroupDocs.Conversion you will be able to convert a multitude of document formats with the possibility to specify different options.

This web application allows you to convert documents between different formats using simple UI. While it can be used as a standalone application it also can be integrated as part of your project.

**Note:** without a license application will run in trial mode, purchase [GroupDocs.Conversion for Java license](https://purchase.groupdocs.com/order-online-step-1-of-8.aspx) or request [GroupDocs.Conversion for Java temporary license](https://purchase.groupdocs.com/temporary-license).

| Supported file formats |
| ---------------------- |
| Bmp                    |
| Csv                    |
| Doc                    |
| Docm                   |
| Docx                   |
| Dot                    |
| Dotm                   |
| Dotx                   |
| Gif                    |
| Htm                    |
| Html                   |
| Ico                    |
| Jpeg                   |
| Jpg                    |
| Odp                    |
| Ods                    |
| Odt                    |
| Ott                    |
| Pdf                    |
| Png                    |
| Pps                    |
| Ppsx                   |
| Ppt                    |
| Pptx                   |
| Psd                    |
| Rtf                    |
| Tif                    |
| Tiff                   |
| Txt                    |
| Xls                    |
| Xls2003                |
| Xlsb                   |
| Xlsm                   |
| Xlsx                   |
| Xps                    |

## Demo Video
Coming soon


## Features
#### GroupDocs.Conversion
- Clean, modern and intuitive design
- Easily switchable colour theme (create your own colour theme in 5 minutes)
- Responsive design
- Convert individual documents
- Batch convert multiple files
- Mobile support (open application on any mobile device)
- HTML and image modes
- Convert documents
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
curl -J -L -o release.tar.gz https://github.com/groupdocs-conversion/GroupDocs.Conversion-for-Java-Spring/releases/download/0.0.1/release.tar.gz
tar -xvzf release.tar.gz
cd release
java -jar Conversion-spring-0.0.1.jar configuration.yaml
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