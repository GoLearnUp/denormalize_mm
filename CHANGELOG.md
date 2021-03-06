# Change Log
All notable changes to this project will be documented in this file.
This project adheres to [Semantic Versioning](http://semver.org/).

## [0.3.1] - 2015-04-08

### Fixed
- Reverse denormalization now plays nicely with TimeWithZone objects.

## [0.3.0] - 2015-03-26

### Changed
- Renamed `#denormalize_association` option `:on` to `:method`. This
  better represents how this is used. The default value is still
  `:before_validation`.

### Added
- The `#denormalize_association` option now accepts parameters `:on`,
  `:if`, `:unless` and `:prepend` and passes those options to the
  validation method call. See `ActiveModel::Validations::ClassMethods`
  and its constant `VALID_OPTIONS_FOR_VALIDATE`.

[0.3.1]: https://github.com/GoLearnUp/fixturize/compare/v0.3.0...0.3.1
[0.3.0]: https://github.com/GoLearnUp/fixturize/compare/v0.2.3...0.3.0
