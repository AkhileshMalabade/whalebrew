# Change log

## 0.2.2 - 2019-07-08
### Fixed
* Whalebrew releases should now be deployed by travis

## 0.2.1 - 2019-07-08
### Fixed
* Whalebrew install not working when registry name was provided

## 0.2.0 - 2019-06-10
### Added
* Use the --init docker flag when running the image, allowing signal management inside the image
* Support for custom hooks for before and after installing or uninstalling a package
* Freeze dependencies with go modules
* Add support to override an image entrypoint
* Add a filter to specify the version of whalebrew required in a package
* Allow customizing the behaviour when volumes are missing

### Fixed
* Docker image build
* Updated docker library using outdated features

### Removed
* internal `run` command is not exposed as a command any longer

## 0.1.0 - 2017-03-23
### Added
* A label for setting the working directory inside the container.
* The ability to put environment variables in `working_dir`, `volumes`, and `environment` labels that are resolved at runtime.
* A `-y` flag to install to assume the answer "yes" to any questions asked.

## 0.0.5 - 2017-03-04
### Added
* Ask permission before installing a package that needs to listen on ports, access environment variables, or access files/directories on the host.
* A `-f` flag to `whalebrew install` to force install a package over an existing file.

## 0.0.4 - 2017-02-07
### Added
* `whalebrew edit` command for editing packages

### Fixed
* Files being written as root

## 0.0.3 - 2017-01-30
### Fixed

* Permission errors when running `whalebrew list`

## 0.0.2 - 2017-01-28
### Added

* Support for mapping ports.

### Fixed

* `whalebrew list` when install path contains folders.

## 0.0.1 - 2017-01-26

Initial release.
