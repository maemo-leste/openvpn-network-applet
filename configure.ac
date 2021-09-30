AC_PREREQ[(2.69)]
AC_INIT([openvpn-network-applet], [0.1], [parazyd@dyne.org])
AM_INIT_AUTOMAKE
AC_CONFIG_HEADER([config.h])
AC_CONFIG_MACRO_DIRS([m4])

AC_PROG_CC
AC_PROG_INSTALL
AM_PROG_LIBTOOL

PKG_CHECK_MODULES(libhildon, hildon-1)
PKG_CHECK_MODULES(libhildonfm, hildon-fm-2)
PKG_CHECK_MODULES(libhildondesktop, libhildondesktop-1)
PKG_CHECK_MODULES(hildoncontrolpanel, hildon-control-panel)
PKG_CHECK_MODULES(gtk2, gtk+-2.0)
PKG_CHECK_MODULES(glib2, glib-2.0)
PKG_CHECK_MODULES(libosso, libosso)
PKG_CHECK_MODULES(gconf, gconf-2.0)
PKG_CHECK_MODULES(dbus, dbus-1)

icon48dir=`pkg-config libhildondesktop-1 --variable=prefix`/share/icons/hicolor/48x48/hildon
icon18dir=`pkg-config libhildondesktop-1 --variable=prefix`/share/icons/hicolor/18x18/hildon

hildonhomedesktopdir=`pkg-config libhildondesktop-1 --variable=hildonstatusmenudesktopentrydir`
hildondesktoplibdir=`pkg-config libhildondesktop-1 --variable=hildondesktoplibdir`

controlpaneldesktopdir=`pkg-config hildon-control-panel --variable=plugindesktopentrydir`
controlpanellibdir=`pkg-config hildon-control-panel --variable=pluginlibdir`

AC_SUBST(libhildon_CFLAGS)
AC_SUBST(libhildon_LIBS)
AC_SUBST(libhildonfm_CFLAGS)
AC_SUBST(libhildonfm_LIBS)
AC_SUBST(libhildondesktop_CFLAGS)
AC_SUBST(libhildondesktop_LIBS)
AC_SUBST(gtk2_CFLAGS)
AC_SUBST(gtk2_LIBS)
AC_SUBST(glib2_CFLAGS)
AC_SUBST(glib2_LIBS)
AC_SUBST(libosso_CFLAGS)
AC_SUBST(libosso_LIBS)
AC_SUBST(gconf_CFLAGS)
AC_SUBST(gconf_LIBS)
AC_SUBST(dbus_CFLAGS)
AC_SUBST(dbus_LIBS)
AC_SUBST(icon48dir)
AC_SUBST(icon18dir)
AC_SUBST(hildonhomedesktopdir)
AC_SUBST(hildondesktoplibdir)
AC_SUBST(controlpaneldesktopdir)
AC_SUBST(controlpanellibdir)

AC_OUTPUT([
	Makefile
	status-applet/Makefile
	control-applet/Makefile
	data/Makefile
])
