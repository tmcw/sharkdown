[![Build Status](https://secure.travis-ci.org/tmcw/sharkdown.png?branch=master)](http://travis-ci.org/tmcw/sharkdown)

# sharkdown

## usage

    npm install --save sharkdown

## api

### `sharkdown(str)`

Takes a string, returns a string with markdown encoded as control codes for a
shell.

### `sharkdown()`

Returns a through-stream for pipes.

## example

    process.stdin.pipe(sharkdown()).pipe(process.stdout);