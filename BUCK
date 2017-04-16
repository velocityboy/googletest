cxx_library(
  name = 'gtest',
  srcs = [
   'googletest/src/gtest-all.cc',
   'googlemock/src/gmock-all.cc',
   'googlemock/src/gmock_main.cc',
  ],
  header_namespace = '',
  exported_headers = subdir_glob([
    ('googletest/include', '**/*.h'),
    ('googlemock/include', '**/*.h'),
  ]),
  headers = subdir_glob([
    ('googletest', 'src/*.cc'),
    ('googletest', 'src/*.h'),
    ('googlemock', 'src/*.cc'),
    ('googlemock', 'src/*.h'),
  ]),
  platform_linker_flags = [
    ('', ['-lpthread']),
  ],
  visibility = [
    '//test/...',
  ],
)
