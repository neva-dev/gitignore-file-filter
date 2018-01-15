![Neva Development logo](docs/neva-logo.png)

[![Gradle Status](https://gradleupdate.appspot.com/Cognifide/gradle-aem-plugin/status.svg)](https://gradleupdate.appspot.com/Cognifide/gradle-aem-plugin/status)
[![Apache License, Version 2.0, January 2004](https://img.shields.io/github/license/Cognifide/gradle-aem-plugin.svg?label=License)](http://www.apache.org/licenses/)

# GitIgnore File Filter


## Description

It is a reusable wrapper for file exclusion mechanism extracted from [NetBeans Git Module](https://github.com/myabc/nbgit/tree/master/src/org/nbgit/util/exclude).


## Usage

```kotlin
val rootDir = File("/some/root")
val sampleFile = File("SomeClass.class", rootDir)
val gitIgnore = GitIgnore(rootDir)

if (gitIgnore.isExcluded(sampleFile)) {
    // ...
}
```

## License

**GitIgnore File Filter** is licensed under the [Apache License, Version 2.0 (the "License")](https://www.apache.org/licenses/LICENSE-2.0.txt)
