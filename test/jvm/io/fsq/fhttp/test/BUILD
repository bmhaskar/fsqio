# Copyright 2015 Foursquare Labs Inc. All Rights Reserved.

junit_tests(
  name = 'test',
  sources = globs('*.scala'),
  dependencies = [
    '3rdparty:finagle',
    '3rdparty:junit',
    '3rdparty:netty',
    '3rdparty:twitter-util',
    'src/jvm/io/fsq/fhttp',
  ],
  # NOTE(mateo): These tests appear to not be threadsafe. They fail when ran with any type of concurrency.
  concurrency="SERIAL",
)
