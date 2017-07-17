# ruby-with-therubyracer

Inspired by https://github.com/teradiot/alpine-ruby-libv8

## Example

```
$ docker run --rm usualoma/ruby-with-therubyracer:2.4.1-alpine ruby -e 'require "v8"; puts V8::Context.new.eval("7 * 6")'
42
```
