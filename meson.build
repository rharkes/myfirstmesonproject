project('purelib-and-platlib', 'c')

py = import('python').find_installation(pure: false)

py.extension_module(
    'mycmodule',
    'src/mycmodule/mycmodule.c',
    install: true,
)

install_subdir('src/mypythonmodule', install_dir : py.get_install_dir(pure: false))