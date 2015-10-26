#Play Language Support Plugin

[![Apache-2.0 license](http://img.shields.io/badge/license-Apache-brightgreen.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)

[![Build Status](https://travis-ci.org/hmrc/play-language.svg)](https://travis-ci.org/hmrc/play-language-support) [ ![Download](https://api.bintray.com/packages/hmrc/releases/play-language-support/images/download.svg) ](https://bintray.com/hmrc/releases/play-language/_latestVersion)


Plugin to provide common language support and switching functionality for Play +2.2.3 projects.

##Endpoints

This adds two endpoints:

```
     /switch-to-english     - Switches the current language to English
	 /switch-to-welsh 		- SWitches the current language to Welsh
```

##Setup

Add the jar to the projects dependencies:

```
    "uk.gov.hmrc" %% "play-language-support" % "[INSERT VERSION]"
```

Add plugin to play.plugins:

```
    {priority}:uk.gov.hmrc.play.language.LanguagePlugin
```

Additionally, add the following to the routes file:

```
    ->     /                                    language.Routes
```

## Configuration

The plugin expects to find the apps name in the `application.conf` under the key `appName`.

## License ##
 
This code is open source software licensed under the [Apache 2.0 License]("http://www.apache.org/licenses/LICENSE-2.0.html").