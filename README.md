# restful-api-sorter
Utilities for sorting go-restful api's for output in Swagger

## Description

If you utilize [go-restful](https://github.com/emicklei/go-restful)'s ability to generate [Swagger](http://swagger.io/)
docs, you've undoutedly noticed that the order is not pre-defined and must be sorted client-side.  This can be
problematic if you have a particularly large API list.

To that end, this package endeavors to sort the api's in go, which is just better.

## Available Sort Methods

- [AscendingByResourcePath](./sorters#L8)
