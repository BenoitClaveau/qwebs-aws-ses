# qwebs-aws-ses
[AWS SES](https://aws.amazon.com/documentation/ses/) service for [Qwebs server](https://www.npmjs.com/package/qwebs).

 [![NPM][npm-image]][npm-url]
 [![Build Status][travis-image]][travis-url]
 [![Coverage Status][coveralls-image]][coveralls-url]

## Features

  * [Qwebs](https://www.npmjs.com/package/qwebs)
  * [AWS SES API](http://docs.aws.amazon.com/ses/latest/DeveloperGuide/send-email-api.html)


## AWS SES

```config.json
{
    "aws": {
        "ses": {
            "apiVersion": "2010-12-01", 
            "region": "eu-west-1",
        }
    }
}
```

### Declare and inject AWS SES service

```routes.json
{
  "services": [
    { "name": "$aws-ses", "location": "qwebs-aws-ses" }
  ]
}
```

## Installation

```bash
$ npm install qwebs-aws-ses
```

## Test

To run our tests, clone the qwebs-aws-ses repo and install the dependencies.

```bash
$ git clone https://github.com/BenoitClaveau/qwebs-aws-ses --depth 1
$ cd qwebs-aws-ses
$ npm install
$ node.exe "..\node_modules\jasmine-node\bin\jasmine-node" --verbose tests
```

[npm-image]: https://img.shields.io/npm/v/qwebs-aws-ses.svg
[npm-url]: https://npmjs.org/package/qwebs-aws-ses
[travis-image]: https://travis-ci.org/BenoitClaveau/qwebs-aws-ses.svg?branch=master
[travis-url]: https://travis-ci.org/BenoitClaveau/qwebs-aws-ses
[coveralls-image]: https://coveralls.io/repos/BenoitClaveau/qwebs-aws-ses/badge.svg?branch=master&service=github
[coveralls-url]: https://coveralls.io/github/BenoitClaveau/qwebs-aws-ses?branch=master
