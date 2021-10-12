# aqovia-openapi-generator-cli

<i>*** This is a fork of @openapitools/openapi-generator-cli (v4.3.0) - with the addition of a C# Azure Functions server generator ***</i>

---

OpenAPI Generator allows generation of API client libraries (SDK generation), server stubs, documentation and 
configuration automatically given an OpenAPI Spec (both 2.0 and 3.0 are supported). Please see
[OpenAPITools/openapi-generator](https://github.com/OpenAPITools/openapi-generator)

---

**Thanks [openapitools.org](https://openapitools.org) for this awesome CLI!**

## Installation

There are several ways to install the package.

#### Global Mode

In global mode (ie, with -g or --global appended to the command), it installs the package as a global package. This 
means that you'll get the `openapi-generator` command available on your command line interface (CLI) as well.

```sh
# install the latest version of "aqovia-openapi-generator-cli"
npm install aqovia-openapi-generator-cli -g
```

After the installation has finished you can type for example:

```sh
# this shall print the correct version number
openapi-generator version
```

#### Package Mode

It is recommended to install the package as development dependency, because normally you only need this dependency
during the development process. To do that you can type the following:

```sh
# install the latest version of "aqovia-openapi-generator-cli"
npm install @openapitools/openapi-generator-cli -D
```

After the installation has finished you can add a script like this:

```json
{
  "name": "my-cool-package",
  "version": "0.0.0",
  "scripts": {
    "my-awesome-script-name": "openapi-generator generate -i docs/openapi.yaml -g csharp-netcore-functions -o generated-sources/openapi --additional-properties packageName=MyCoolApi",
  }
}
```

## Further Documentation

Please refer to the [official openapi-generator docs](https://github.com/OpenAPITools/openapi-generator#3---usage) for
more information about the possible arguments and a detailed usage manual of the command line interface.
