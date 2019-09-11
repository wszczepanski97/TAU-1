# TAU

The TAU library contains components which allows you to create Web Application UI. Each components represents UI element, such as a button or slider, which gives you interaction and manipulation features.

This is replacement and clone of previously existing https://review.tizen.org/gerrit/#/admin/projects/platform/framework/web/tau

## Getting Started

- Clone a copy of the master branch in the TAU Git repository:

`git clone git@github.com:Samsung/TAU.git`

- Change to the tau directory:

`cd TAU`

- Check out the latest stable version of TAU:

`git checkout master`

### Prerequisites

To build a TAU library, ensure that you have both Git and Node.js (6.16.0) installed.

Example of node install using [`nvm`](https://github.com/creationix/nvm):

```
nvm install 6.16.0
nvm use 6.16.0
```

### Installing

- Install the build module by npm:

`npm install`

Build TAU by running the following command in the tau directory:

`npx grunt build`

## Running the tests

TAU has automated tests. To run tests execute command:

`npx grunt test`

## Debuggging

In order to set additional logging in TAU you need to build TAU with --tau-debug option

`npx grunt build --tau-debug`

## Demo application:

UIComponents sample web application demonstrating how to implement UI Components for wearable based on TAU.

Demo application is available on https://samsung.github.io/TAU: 

- https://samsung.github.io/TAU/examples/mobile/UIComponents/ (Mobile)
- https://samsung.github.io/TAU/examples/wearable/UIComponents/ (Wearable)

If you want to test your own version of demo app it is available under following paths in repository:

* mobile: `examples\mobile\UIComponents`
* wearable: `examples\wearable\UIComponents`

In order to test it:

- Install http-server in TAU directory

`npm install http-server -g`

- Launch server in TAU directory:

`npx http-server -p <port> -a localhost`

e.g. `npx http-server -p 8888 -a localhost`

- Visit appropriate site:

`http://localhost:PORT/examples/PROFILE/UIComponents/`

e.g.

* http://localhost:8888/examples/wearable/UIComponents/
* http://localhost:8888/examples/mobile/UIComponents/

### Coding style tests

Project has defined eslint rules (.eslintrc.js)

Contribution can be verified using command:

`npx grunt eslint`

## Usage

Refer to [samsung.github.io/TAU](https://samsung.github.io/TAU/) for library usage instructions

## Contributing

Please read [CONTRIBUTING.md](https://github.com/Samsung/TAU/blob/master/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning
TAU version comply with [Semantic Versioning specification - 2.0](https://semver.org/spec/v2.0.0.html)

*MAJOR.MINOR.PATCH*

- *MAJOR* - assures public API compatibility
- *MINOR* - adds new functionalities (e.g. new API) with backward compatibility for old API
- *PATCH* - backward compatible bug fixes

## TAU vs Tizen compatibility
TAU library dedicated Tizen platform version.
- If you use Tizen 4.0/Tizen 5.0, we recommend you use the TAU 1.0.x
- If you use Tizen 5.5, we recommend you use the TAU 1.1.x .


## Releases
You can find releases in the releases [tab](https://github.com/Samsung/TAU/releases)

**Tizen_version_number.TAU_version_for_given_Tizen_release.**

-  In case of TAU for Tizen 4.0: TAU 1.0.1 , TAU 1.0.2, TAU 1.0.3 ...
-  In case of TAU for Tizen 5.5: TAU 1.1.1 , TAU 1.1.2, TAU 1.1.3 ...

## Authors

* Authors - [AUTHOR](https://github.com/Samsung/TAU/blob/master/AUTHOR)

See also the list of [contributors](https://github.com/SAMSUNG/TAU/contributors) who participated in this project.

## License

This project is licensed under MIT except some files under Flora license. For details see [COPYING](https://github.com/Samsung/TAU/blob/master/COPYING)
