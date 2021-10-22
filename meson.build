project(
  'sndfilter',
  'c',
)

sndfilter_lib = library(
  'sndfilter',
  include_directories: include_directories('include'),
  c_args: [
    '-D_USE_MATH_DEFINES' # M_PI, M_LN2
  ],
  sources: files(
    'src/biquad.c',
    'src/compressor.c',
    'src/main.c',
    'src/mem.c',
    'src/reverb.c',
    'src/snd.c',
    'src/wav.c',
  ),
  link_args: [
    '-lm',
    ]
)

sndfilter_dep = declare_dependency(
  link_with: sndfilter_lib,
  include_directories: include_directories('include'),
  link_args: [
    '-lm',
  ]
)
