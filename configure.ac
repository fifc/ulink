AC_PREREQ(2.69)
AC_INIT([ulink], [1.0], [y@ffox.top])
AC_CONFIG_HEADERS([config.h])
dnl AM_INIT_AUTOMAKE([-Wall -Werror foreign])
AC_CONFIG_MACRO_DIRS([m4])
AM_INIT_AUTOMAKE([-Wall -Werror])
AC_PROG_CC
AC_PROG_CXX
AM_PROG_AR
AM_PROG_CC_C_O

LT_INIT

AC_ARG_VAR([PKG_DIR], [pkg dir])
[
if [[ -n "${PKG_DIR}" ]]; then
	CPPFLAGS+=-I${PKG_DIR}/include
	LDFLAGS+=-L${PKG_DIR}/lib
fi
]

dnl PKG_PROG_PKG_CONFIG
dnl AC_CHECK_LIB([boost_chrono], [sdfs], [], [AC_MSG_ERROR()])
dnl PKG_CHECK_MODULES([grpc], [grpc])
dnl PKG_CHECK_MODULES([protobuf], [protobuf])

AC_CONFIG_FILES([
 makefile
 src/makefile
])
AC_OUTPUT
