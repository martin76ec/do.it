project('com.github.martin76ec.doit', 'vala', 'c')

executable(
    meson.project_name(),
    'src/Application.vala',
    dependencies: [
        dependency('gtk+-3.0')
    ],
    install: true
)

install_data(
    join: paths('data', 'doit.desktop'),
    install_dir: join_paths(get_option('datadir'), 'applications')
    rename: meson.project_name() + '.desktop'
)

install_data(
    join_paths('data', 'hello-again.appdata.xml'),
    install_dir: join_paths(get_option('datadir'), 'metainfo'),
    rename: meson.project_name() + '.appdata.xml'
)