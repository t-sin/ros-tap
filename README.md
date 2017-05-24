# ros-tap

Load your local projects when quicklisp initiallized.

## Installation

Use [roswell](https://github.com/roswell/roswell/).

```
$ ros install t-sin/ros-tap
```

## Usage

```sh
# no local systems
$ ros tap list
$ ros run -e "(ql:quickload :rosa)"  # error

# add local system
$ ros tap tap ~/code/rosa/rosa.asd
$ ros tap list
/home/t-sin/code/rosa/rosa.asd
$ ros run -e "(ql:quickload :rosa)"  # loaded

# delete local system
$ ros tap untap ~/code/rosa/rosa.asd
$ ros tap list
```

## Author

- Shinichi Tanaka (shinichi.tanaka45@gmail.com)

## Copyright

Copyright (c) 2017 Shinichi TANAKA (shinichi.tanaka45@gmail.com)

## License

Licensed under the MIT License.
