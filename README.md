# restful-api-sorter
Utilities for sorting go-restful api's for output in Swagger

## Targeted Versions

| restful-api-sorter | compatibility |
| :---: | :---: |
| [v1.2](https://github.com/myENA/restful-api-sorter/tree/v1.2) | [go-restful v1.2](https://github.com/emicklei/go-restful/tree/v1.2) |
| [swagger12](https://github.com/myENA/restful-api-sorter/tree/swagger12) | [go-restful-swagger12 1.*](https://github.com/emicklei/go-restful-swagger12/tree/1.0.1) |

## Description

If you utilize [go-restful](https://github.com/emicklei/go-restful) or [go-restful-swagger12](https://github.com/emicklei/go-restful-swagger12)'s ability to generate [Swagger](http://swagger.io/)
docs, you've undoutedly noticed that the order is not pre-defined and must be sorted client-side.  This can be
problematic if you have a particularly large API list.

To that end, this package endeavors to sort the api's in go, which is just better.

## Available Sort Methods

- [AscendingByResourcePath](./sorters.go#L8)

## Usage

Each of the functions present in this package are implementations of 
[PostBuildDeclarationMapFunc](https://github.com/emicklei/go-restful/blob/v1.2/swagger/config.go#L10), and is used
by setting the `PostBuildHandler` property on the 
[Config](https://github.com/emicklei/go-restful/blob/v1.2/swagger/config.go#L12) struct.
