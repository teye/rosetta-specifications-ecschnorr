# Rosetta Specifications

[![Coinbase](https://circleci.com/gh/coinbase/rosetta-specifications/tree/master.svg?style=shield)](https://circleci.com/gh/coinbase/rosetta-specifications/tree/master)
[![License](https://img.shields.io/github/license/coinbase/rosetta-specifications.svg)](https://github.com/coinbase/rosetta-specifications/blob/master/LICENSE.txt)

## What is Rosetta?
Rosetta is a new project from Coinbase to standardize the process
of deploying and interacting with blockchains. With an explicit
specification to adhere to, all parties involved in blockchain
development can spend less time figuring out how to integrate
with each other and more time working on the novel advances that
will push the blockchain ecosystem forward. In practice, this means
that any blockchain project that implements the requirements outlined
in this specification will enable exchanges, block explorers,
and wallets to integrate with much less communication overhead
and network-specific work.

## Specifications
This repository contains all specification files used to generate code for the
Rosetta API. The Rosetta API is specified in the [OpenAPI 3.0 format](https://www.openapis.org)
(the [successor to Swagger/OpenAPI 2.0](https://swagger.io/blog/news/whats-new-in-openapi-3-0)).
Requests and responses can be crafted with autogenerated code using
[Swagger Codegen](https://swagger.io/tools/swagger-codegen) or
[OpenAPI Generator](https://openapi-generator.tech) (with
the downloadable JSON spec at the top of this site),
are human-readable (easy to debug and understand), and can be used in servers and browsers.

Check out the [rosetta-sdk-go](https://github.com/coinbase/rosetta-sdk-go)
repository for an example of how to generate code using this specification.

## Development
* `make deps` to install dependencies
* `make gen` to generate the specification files
* `make validate` to ensure specification is valid
* `make release` to check if code passes all tests run by CircleCI

## Future Work
* Wallet API for standard construction and signing of transactions

## License
This project is available open source under the terms of the [Apache 2.0 License](https://opensource.org/licenses/Apache-2.0).

© 2020 Coinbase
