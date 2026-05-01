project(
    'jiggy',
    ['c','cpp'],
    version: '1.0',
    license: 'GPL',
    default_options: ['warning_level=2', 'unity=off','buildtype=debug'],
    meson_version: '>= 1.1',
)

subdir('targets/radrr')
subdir('targets/iggy')

lib = shared_library(
    'jiggy',
    sources,
    version: '1.0.0',
        dependencies: [
          iggy_dep
    ]
)

# Iggy utilizes stb_truetype so while it's unused right now
# The subproject is set up for later

# MARK: TESTS
pymod = import('python')
python = pymod.find_installation('python3', required: true)
test_files = files()

foreach test_file : test_files
    test('test', python, args: [test_file])
endforeach
