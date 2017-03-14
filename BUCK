cxx_library(
  name = 'util',
  header_namespace = 'util',
  exported_headers = subdir_glob([
    ('util', '**/*.h'),
  ]),
  srcs = glob([
    'util/**/*.cc',
  ], excludes = glob([
    'util/**/*_unittest.cc',
  ])),
)

cxx_library(
  name = 'compact-enc-det',
  header_namespace = 'compact_enc_det',
  exported_headers = subdir_glob([
    ('compact_enc_det', '*.h'),
  ]),
  srcs = glob([
    'compact_enc_det/*.cc',
  ], excludes = glob([
    'compact_enc_det/*_unittest.cc',
    'compact_enc_det/*_test.cc',
  ])),
  visibility = [
    'PUBLIC',
  ],
  deps = [
    ':util',
  ],
)
