project('littlefs', 'c',
        version: '2.4.0',
        license: 'BSD-3-Clause')

littlefs_inc = include_directories('.')
littlefs_lib = static_library('littlefs', [
                               'lfs.c',
                               'lfs_util.c',
                             ],
                              pic: false)

littlefs_dep = declare_dependency(link_with: littlefs_lib,
                                  include_directories: littlefs_inc)
