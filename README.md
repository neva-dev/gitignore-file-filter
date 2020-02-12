![Neva Development logo](docs/neva-logo.png)

[![Download](https://api.bintray.com/packages/neva-dev/maven-public/gitignore-file-filter/images/download.svg) ](https://bintray.com/neva-dev/maven-public/gitignore-file-filter/_latestVersion)
[![Gradle Status](https://gradleupdate.appspot.com/Cneva-dev/gitignore-file-filter/status.svg?random=123)](https://gradleupdate.appspot.com/neva-dev/gitignore-file-filter/status)
[![Apache License, Version 2.0, January 2004](docs/apache-license-badge.svg)](http://www.apache.org/licenses/)

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
