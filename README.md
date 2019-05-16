# GroupDocs.Conversion for Java Spring Example
New GroupDocs.Conversion for Java Spring UI Example
###### version 1.9.11

[![Build Status](https://travis-ci.org/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Spring.svg?branch=master)](https://travis-ci.org/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Spring)
[![Maintainability](https://api.codeclimate.com/v1/badges/f945b8bc09a5ff2e8a2d/maintainability)](https://codeclimate.com/github/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Spring/maintainability)
[![GitHub license](https://img.shields.io/github/license/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Spring.svg)](https://github.com/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Spring/blob/master/LICENSE)

## System Requirements
- Java 8 (JDK 1.8)
- Maven 3


## Compare documents with Java API

**GroupDocs.Conversion for Java** is a library that allows you to **compare PDF, DOCX, PPT, XLS,** and over 90 other document formats. With GroupDocs.Conversion for Java you will be able to compare two or more files, perform style and text Conversion and generate a detailed report with changes.

This application allows you to compare multiple documents and can be used as a standalone application or integrated as part of your project.

**Note:** without a license application will run in trial mode, purchase [GroupDocs.Conversion for Java license](https://purchase.groupdocs.com/order-online-step-1-of-8.aspx) or request [GroupDocs.Conversion for Java temporary license](https://purchase.groupdocs.com/temporary-license).


## Demo Video
Coming soon


## Features
#### GroupDocs.Conversion
- Clean, modern and intuitive design
- Easily switchable colour theme (create your own colour theme in 5 minutes)
- Responsive design
- Mobile support (open application on any mobile device)
- HTML and image modes
- Fully customizable navigation panel
- Compare documents
- Multi-compare several documents
- Compare password protected documents
- Upload documents
- Display clearly visible differences
- Download Conversion results
- Print Conversion results
- Smooth document scrolling
- Preload pages for faster document rendering
- Multi-language support for displaying errors
- Cross-browser support (Safari, Chrome, Opera, Firefox)
- Cross-platform support (Windows, Linux, MacOS)


## How to run

You can run this sample by one of following methods


#### Build from source

Download [source code](https://github.com/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Spring/archive/master.zip) from github or clone this repository.

```bash
git clone https://github.com/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Spring
cd GroupDocs.Conversion-for-Java-Spring
mvn clean spring-boot:run
## Open http://localhost:8080/Conversion/ in your favorite browser.
```

#### Build war from source

Download [source code](https://github.com/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Spring/archive/master.zip) from github or clone this repository.

```bash
git clone https://github.com/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Spring
cd GroupDocs.Conversion-for-Java-Spring
mvn package -P war
## Deploy this war on any server
```

#### Binary release (with all dependencies)

Download [latest release](https://github.com/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Spring/releases/latest) from [releases page](https://github.com/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Spring/releases). 

**Note**: This method is **recommended** for running this sample behind firewall.

```bash
curl -J -L -o release.tar.gz https://github.com/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Spring/releases/download/1.9.11/release.tar.gz
tar -xvzf release.tar.gz
cd release
java -jar Conversion-spring-1.9.11.jar configuration.yaml
## Open http://localhost:8080/Conversion/ in your favorite browser.
```

#### Docker image
Use [docker](https://hub.docker.com/u/groupdocs) image.

```bash
mkdir DocumentSamples
mkdir Licenses
docker run -p 8080:8080 --env application.hostAddress=localhost -v `pwd`/DocumentSamples:/home/groupdocs/app/DocumentSamples -v `pwd`/Licenses:/home/groupdocs/app/Licenses groupdocs/Conversion
## Open http://localhost:8080/Conversion/ in your favorite browser.
```

## Configuration
For all methods above you can adjust settings in `configuration.yml`. By default in this sample will lookup for license file in `./Licenses` folder, so you can simply put your license file in that folder or specify relative/absolute path by setting `licensePath` value in `configuration.yml`. 

### Conversion configuration options

| Option                             | Type    |   Default value   | Description                                                                                                                                  |
| ---------------------------------- | ------- |:-----------------:|:-------------------------------------------------------------------------------------------------------------------------------------------- |
| **`filesDirectory`**               | String  | `DocumentSamples` | Files directory path. Indicates where uploaded and predefined files are stored. It can be absolute or relative path                          |
| **`fontsDirectory`**               | String  |                   | Path to custom fonts directory.                                                                                                              |
| **`defaultDocument`**              | String  |                   | Absolute path to default document that will be loaded automaticaly.                                                                          |
| **`preloadPageCount`**             | Integer |        `0`        | Indicate how many pages from a document should be loaded, remaining pages will be loaded on page scrolling.Set `0` to load all pages at once |
| **`multiComparing`**               | String  |      `true`       | Enable/disable multi comparing feature                                                                                                       |

## License
The MIT License (MIT). 

Please have a look at the LICENSE.md for more details

## GroupDocs Conversion on other platforms & frameworks

- [Comapre documents](https://github.com/groupdocs-Conversion/GroupDocs.Conversion-for-Java-Dropwizard) with JAVA Dropwizard 
- [Comapre documents](https://github.com/groupdocs-Conversion/GroupDocs.Conversion-for-.NET-MVC) with .NET MVC 
- [Comapre documents](https://github.com/groupdocs-Conversion/GroupDocs.Conversion-for-.NET-WebForms) with .NET WebForms 


## Resources
- **Website:** [www.groupdocs.com](http://www.groupdocs.com)
- **Product Home:** [GroupDocs.Conversion for Java](https://products.groupdocs.com/Conversion/java)
- **Product API References:** [GroupDocs.Conversion for Java API](https://apireference.groupdocs.com)
- **Download:** [Download GroupDocs.Conversion for Java](http://downloads.groupdocs.com/Conversion/java)
- **Documentation:** [GroupDocs.Conversion for Java Documentation](https://docs.groupdocs.com/dashboard.action)
- **Free Support Forum:** [GroupDocs.Conversion for Java Free Support Forum](https://forum.groupdocs.com/c/Conversion)
- **Paid Support Helpdesk:** [GroupDocs.Conversion for Java Paid Support Helpdesk](https://helpdesk.groupdocs.com)
- **Blog:** [GroupDocs.Conversion for Java Blog](https://blog.groupdocs.com/category/groupdocs-Conversion-product-family)