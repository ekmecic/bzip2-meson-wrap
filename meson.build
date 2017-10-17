project('bzip2', 'c', version: '1.0.6')

bzip2_src = [
  'bzlib.h'
  'bzlib_private.h'
  'blocksort.c',
  'huffman.c',
  'crctable.c',
  'randtable.c',
  'compress.c',
  'decompress.c',
  'bzlib.c']

bzip2_incs = include_directories('.')

static_library('bzip2'
               sources: bzip2_src,
               include_directories: bzip2_incs)

bzip2_dep = declare_dependency(link_with: bzip2, include_directories: bzip2_incs)
