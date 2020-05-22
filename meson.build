project(
  'ukui-wallpapers',
  version: '20.04.2'
)

i18n = import('i18n')

po_dir = join_paths(meson.source_root(), 'po')
its_dir = join_paths(meson.source_root(), 'gettext')

install_subdir(
  'backgrounds',
  install_dir: get_option('datadir'),
)

ukui_background_dir = join_paths(get_option('datadir'), 'ukui-background-properties')
i18n.merge_file(
  input: 'ukui-wallpapers.xml.in',
  output: 'ukui-wallpapers.xml',
  po_dir: po_dir,
  data_dirs: its_dir,
  install: true,
  install_dir: ukui_background_dir,
)

subdir('po')
