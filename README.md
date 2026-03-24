### CommonAPI C++ SOME/IP Tools

##### Copyright
Copyright (C) 2015-2023, Bayerische Motoren Werke Aktiengesellschaft (BMW AG).
Copyright (C) 2015-2023, COVESA

This file is part of COVESA Project IPC Common API C++.
Contributions are licensed to the COVESA under one or more Contribution License Agreements or MPL 2.0.

##### License
This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed with this file, you can obtain one at http://mozilla.org/MPL/2.0/.

##### CommonAPI C++ Specification and User Guide
The specification document and the user guide can be found in the CommonAPI documentation directory of the CommonAPI-Tools project.

##### Further information
https://covesa.github.io/capicxx-core-tools/

##### Dependencies

This project requires **CommonAPI C++ Core Tools** (capicxx-core-tools) as a build-time dependency.

###### Dependency Matrix

The following table shows which versions of someip-tools are built with which versions of core-tools:

| SomeIP Tools Version | Core Tools Version | Notes |
|---------------------|-------------------|-------|
| v3.3.1             | v3.3.1     | Current development version |

> **Note**: When core-tools is updated to a new version, this repository follows these guidelines:
> - **No changes needed in someip-tools code** if the update is compatible
> - A new release of someip-tools will be created to track the dependency update
> - The dependency version is documented in release notes

##### Build Instructions for Linux

You can build all code generators by calling maven from the command-line. Open a console and change in the directory org.genivi.commonapi.someip.releng of your CommonAPI-Tools directory. Then call:

```bash
mvn -DCOREPATH=<path to your CommonAPI-Tools dir> -Dtarget.id=org.genivi.commonapi.someip.target clean verify
```
_COREPATH_ is the directory, that contains the target definition folder: `org.genivi.commonapi.someip.target`.

After the successful build you will find the commond-line generators archived in `org.genivi.commonapi.someip.cli.product/target/products/commonapi_someip_generator.zip` and the update-sites in `org.genivi.commonapi.someip.updatesite/target`.
