![Neva Development logo](docs/neva-logo.png)

[![Gradle Status](https://gradleupdate.appspot.com/Cognifide/gradle-aem-plugin/status.svg)](https://gradleupdate.appspot.com/Cognifide/gradle-aem-plugin/status)
[![Apache License, Version 2.0, January 2004](https://img.shields.io/github/license/Cognifide/gradle-aem-plugin.svg?label=License)](http://www.apache.org/licenses/)

# GitIgnore File Filter


## Description

It is a reusable Java wrapper for [GitIgnore](https://git-scm.com/docs/gitignore) file exclusion mechanism extracted from [NetBeans Git Module](https://github.com/myabc/nbgit/tree/master/src/org/nbgit/util/exclude).

Useful for Java applications or libraries which wants to use GitIgnore like file filtering. 

Supports nested *.gitignore* files.

## Setup

1) Enter [BinTray](https://bintray.com/neva-dev/maven-public/gitignore-file-filter) and setup repository and compile dependency in project build.
2) Consider sample Kotlin code:

```kotlin
val rootDir = File("/some/root")
val sampleFile = File("class/SomeClass.class", rootDir)
val gitIgnore = GitIgnore(rootDir)

if (gitIgnore.isExcluded(sampleFile)) {
    // ...
}
```

## License

**GitIgnore File Filter** is licensed under the [Apache License, Version 2.0 (the "License")](https://www.apache.org/licenses/LICENSE-2.0.txt)
