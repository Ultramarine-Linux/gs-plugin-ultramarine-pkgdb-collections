project(
  'gs-plugin-ultramarine-pkgdb-collections',
  'c',
  version: '0.1.0'
)

gnome_software_dep = dependency('gnome-software', version: '>=45.0')
plugin_install_dir = gnome_software_dep.get_variable('plugindir')

cargs = [
  '-DG_LOG_DOMAIN="GsPluginUltramarinePkgdbCollections"',
  '-DI_KNOW_THE_GNOME_SOFTWARE_API_IS_SUBJECT_TO_CHANGE'
]

glib_dep = dependency('glib-2.0', version: '>=2.60')
gobject_dep = dependency('gobject-2.0')
gio_dep = dependency('gio-2.0')

shared_module(
  'gs_plugin_ultramarine-pkgdb-collections',
  sources : 'gs-plugin-ultramarine-pkgdb-collections.c',
  install : true,
  install_dir: plugin_install_dir,
  c_args : cargs,
  dependencies : [ gnome_software_dep, glib_dep, gobject_dep, gio_dep ],
)

install_data(
  'data/org.gnome.Software.Plugin.UltramarinePkgdbCollections.metainfo.xml',
  install_dir: join_paths(get_option('datadir'), 'metainfo'),
)
