# Copyright 2015 Foursquare Labs Inc. All Rights Reserved.

junit_tests(
  name = 'test',
  sources = globs('*.scala'),
  dependencies = [
    '3rdparty:junit',
    '3rdparty:mongodb-drivers',
    '3rdparty:specs2',
    'src/jvm/io/fsq/field',
    'src/jvm/io/fsq/rogue',
    'src/jvm/io/fsq/rogue/index',
  ],
  # NOTE(mateo): These tests appear to not be threadsafe. They fail when ran with any type of concurrency.
  concurrency="SERIAL",
)
