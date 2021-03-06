# openapi-java-client

Swagger Employee Service
- API version: 1.0.0
  - Build date: 2019-01-27T05:59:30.325+05:30[Asia/Kolkata]

A sample restful application generated using OpenApiGenerator(https://github.com/OpenAPITools/openapi-generator) and its Gradle plugin (https://github.com/OpenAPITools/openapi-generator/blob/master/modules/openapi-generator-gradle-plugin/README.adoc)


*Automatically generated by the [OpenAPI Generator](https://openapi-generator.tech)*


## Requirements

Building the API client library requires:
1. Java 1.8+
2. Maven/Gradle

## Installation

To install the API client library to your local Maven repository, simply execute:

```shell
mvn clean install
```

To deploy it to a remote Maven repository instead, configure the settings of the repository and execute:

```shell
mvn clean deploy
```

Refer to the [OSSRH Guide](http://central.sonatype.org/pages/ossrh-guide.html) for more information.

### Maven users

Add this dependency to your project's POM:

```xml
<dependency>
  <groupId>org.openapitools</groupId>
  <artifactId>openapi-java-client</artifactId>
  <version>1.0.0</version>
  <scope>compile</scope>
</dependency>
```

### Gradle users

Add this dependency to your project's build file:

```groovy
compile "org.openapitools:openapi-java-client:1.0.0"
```

### Others

At first generate the JAR by executing:

```shell
mvn clean package
```

Then manually install the following JARs:

* `target/openapi-java-client-1.0.0.jar`
* `target/lib/*.jar`

## Getting Started

Please follow the [installation](#installation) instruction and execute the following Java code:

```java

import com.milan.openapi.employee.*;
import com.milan.openapi.employee.auth.*;
import com.milan.openapi.employee.model.*;
import com.milan.openapi.employee.api.EmployeesApi;

import java.io.File;
import java.util.*;

public class EmployeesApiExample {

    public static void main(String[] args) {
        
        EmployeesApi apiInstance = new EmployeesApi();
        try {
            apiInstance.createEmployee();
        } catch (ApiException e) {
            System.err.println("Exception when calling EmployeesApi#createEmployee");
            e.printStackTrace();
        }
    }
}

```

## Documentation for API Endpoints

All URIs are relative to *http://localhost:8081/employee-service*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*EmployeesApi* | [**createEmployee**](docs/EmployeesApi.md#createEmployee) | **POST** /employees | Create an employee
*EmployeesApi* | [**deleteEmployeetById**](docs/EmployeesApi.md#deleteEmployeetById) | **DELETE** /employees/{employeeId} | Delete specific employee
*EmployeesApi* | [**listEmployees**](docs/EmployeesApi.md#listEmployees) | **GET** /employees | List all employees
*EmployeesApi* | [**showEmployeetById**](docs/EmployeesApi.md#showEmployeetById) | **GET** /employees/{employeeId} | Info for a specific employee
*EmployeesApi* | [**updateEmployee**](docs/EmployeesApi.md#updateEmployee) | **PUT** /employees | Update an employee


## Documentation for Models

 - [Employee](docs/Employee.md)
 - [Error](docs/Error.md)


## Documentation for Authorization

All endpoints do not require authorization.
Authentication schemes defined for the API:

## Recommendation

It's recommended to create an instance of `ApiClient` per thread in a multithreaded environment to avoid any potential issues.

## Author



