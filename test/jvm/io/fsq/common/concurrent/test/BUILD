# Copyright 2016 Foursquare Labs Inc. All Rights Reserved.

junit_tests(
  name = 'test',
  sources = globs('*.scala'),
  dependencies = [
    '3rdparty:junit',
    '3rdparty:twitter-util',
    'src/jvm/io/fsq/common/concurrent',
    'src/jvm/io/fsq/common/scala',
  ],
  # NOTE(mateo): These tests appear to not be threadsafe. They fail when ran with any type of concurrency.
  concurrency='SERIAL',
)
