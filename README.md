# module-ballerinax-sap.s4hana.inventory

[![Build](https://github.com/ballerina-platform/module-ballerinax-sap.s4hana.inventory/actions/workflows/ci.yml/badge.svg)](https://github.com/ballerina-platform/module-ballerinax-sap.s4hana.inventory/actions/workflows/ci.yml)
[![codecov](https://codecov.io/gh/ballerina-platform/module-ballerinax-sap.s4hana.inventory/branch/main/graph/badge.svg)](https://codecov.io/gh/ballerina-platform/module-ballerinax-sap.s4hana.inventory)
[![Trivy](https://github.com/ballerina-platform/module-ballerinax-sap.s4hana.inventory/actions/workflows/trivy-scan.yml/badge.svg)](https://github.com/ballerina-platform/module-ballerinax-sap.s4hana.inventory/actions/workflows/trivy-scan.yml)
[![GraalVM Check](https://github.com/ballerina-platform/module-ballerinax-sap.s4hana.inventory/actions/workflows/build-with-bal-test-graalvm.yml/badge.svg)](https://github.com/ballerina-platform/module-ballerinax-sap.s4hana.inventory/actions/workflows/build-with-bal-test-graalvm.yml)
[![GitHub Last Commit](https://img.shields.io/github/last-commit/ballerina-platform/module-ballerinax-sap.s4hana.inventory.svg)](https://github.com/ballerina-platform/module-ballerinax-sap.s4hana.inventory/commits/main)
[![GitHub Issues](https://img.shields.io/github/issues/ballerina-platform/ballerina-library/module/s4hana.svg?label=Open%20Issues)](https://github.com/ballerina-platform/ballerina-library/labels/module%2Fs4hana)

[S/4HANA](https://www.sap.com/india/products/erp/s4hana.html) is a robust enterprise resource planning (ERP) solution,
designed for large-scale enterprises by SAP SE.

This repository encompasses all Ballerina packages pertaining to the S/4HANA inventory submodule. Notably:

## Issues and projects

The **Issues** and **Projects** tabs are disabled for this repository as this is part of the Ballerina library. To
report bugs, request new features, start new discussions, view project boards, etc., visit the Ballerina
library [parent repository](https://github.com/ballerina-platform/ballerina-library).

This repository only contains the source code for the package.

## Build from the source

### Prerequisites

1. Download and install Java SE Development Kit (JDK) version 17. You can download it from either of the following
   sources:

    * [Oracle JDK](https://www.oracle.com/java/technologies/downloads/)
    * [OpenJDK](https://adoptium.net/)

   > **Note:** After installation, remember to set the `JAVA_HOME` environment variable to the directory where JDK was
   installed.

2. Download and install [Ballerina Swan Lake](https://ballerina.io/).

3. Download and install [Docker](https://www.docker.com/get-started).

   > **Note**: Ensure that the Docker daemon is running before executing any tests.

### Build options

Execute the commands below to build from the source.

1. To build all packages:

   ```bash
   ./gradlew clean build
   ```

2. To run the tests in all packages:

   ```bash
   ./gradlew clean test
   ```

3. To build the without the tests:

   ```bash
   ./gradlew clean build -x test
   ```

4. To build only one specific package

   ```bash
   ./gradlew clean :inventory-ballerina:<api_name>:build
   ```

   | API Name                     |            Connector                               |
   | -----------------------------| ---------------------------------------------------|
   | api_material_document_srv    | ballerinax/sap.s4hana.api_material_document_srv    |
   | api_material_stock_srv       | ballerinax/sap.s4hana.api_material_stock_srv       |
   | api_reservation_document_srv | ballerinax/sap.s4hana.api_reservation_document_srv |

5. To run tests against different environment:

   ```bash
   isTestOnLiveServer=true ./gradlew clean test 
   ```
   **Note**: `isTestOnLiveServer` is false by default, tests are run against mock server.

6. To debug packages with a remote debugger:

   ```bash
   ./gradlew clean build -Pdebug=<port>
   ```

7. To debug with the Ballerina language:

   ```bash
   ./gradlew clean build -PbalJavaDebug=<port>
   ```

8. Publish the generated artifacts to the local Ballerina Central repository:

    ```bash
    ./gradlew clean build -PpublishToLocalCentral=true
    ```

9. Publish the generated artifacts to the Ballerina Central repository:

   ```bash
   ./gradlew clean build -PpublishToCentral=true
   ```

## Contribute to Ballerina

As an open-source project, Ballerina welcomes contributions from the community.

For more information, go to
the [contribution guidelines](https://github.com/ballerina-platform/ballerina-lang/blob/master/CONTRIBUTING.md).

## Code of conduct

All the contributors are encouraged to read the [Ballerina Code of Conduct](https://ballerina.io/code-of-conduct).

## Useful links

* For more information go to the [`sap` package](https://lib.ballerina.io/ballerinax/sap/latest).
* For example demonstrations of the usage, go to [Ballerina By Examples](https://ballerina.io/learn/by-example/).
* Chat live with us via our [Discord server](https://discord.gg/ballerinalang).
* Post all technical questions on Stack Overflow with
  the [#ballerina](https://stackoverflow.com/questions/tagged/ballerina) tag.