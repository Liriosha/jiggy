sources = files(
 'src/arithbit.c',
 'src/radarith.c',
 # 'src/radarith_exact.cpp',
 'src/radlz.c',
 'src/rrCore.c',
 'src/rrMath.cpp',
 'src/rrBase.cpp',
 'src/encode.c',
 # 'src/sort.cpp',
 # 'src/contain.cpp',
 'src/wavelet.c'
)

lib_rad = static_library(
    'rad',
    sources,
    include_directories: include_directories('include'),
)

rad_dep = declare_dependency(
    link_with: lib_rad,
    include_directories: include_directories('include'),
)
