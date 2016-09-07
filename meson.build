project('external dependency', 'cpp')

c_args = ['-fpermissive', 
'-Wwrite-strings', 
'-O1',
'-w',
'-fPIC']

inc = include_directories('.')

lib = shared_library('json11', c_args : c_args, include_directories : [inc], sources: 
[
    'json11.cpp'
])

json11_dep = declare_dependency(link_with : lib, 
  include_directories : [inc])
