sources = files(
  'src/allocation.c',
  'src/api_functions.c',
  'src/arena_allocator.c',
  'src/file_reader.c',
  'src/font_provider.c',
  'src/iggy.c',
  'src/main.c',
  'src/sound.c',
  'src/strings.c'
)

lib_iggy = static_library(
    'iggy',
    sources,
    include_directories: include_directories('include', '../rad/include'),
)

iggy_dep = declare_dependency(
    link_with: lib_rad,
    include_directories: include_directories('include', '../rad/include'),
)
