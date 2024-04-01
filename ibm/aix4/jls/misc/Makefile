# @(#)26        1.1  src/bos/usr/lpp/jls/fonts/misc/Makefile, fontKJI, bos411, 9428A410j 3/24/94 08:42:54
#
# COMPONENT_NAME: fontKJI
#
# FUNCTIONS: Japanese Default Fonts
#
# ORIGINS: 27
#
# IBM CONFIDENTIAL -- (IBM Confidential Restricted when
# combined with the aggregated modules for this product)
#                  SOURCE MATERIALS
# (C) COPYRIGHT International Business Machines Corp. 1994
# All Rights Reserved
#
# US Government Users Restricted Rights - Use, duplication or
# disclosure restricted by GSA ADP Schedule Contract with IBM Corp.
#

FONT_LIST = \
	12x24rk.pcf.Z \
	7x14rk.pcf.Z \
	8x16rk.pcf.Z \
	jiskan16.pcf.Z \
	jiskan24.pcf.Z \
	k14.pcf.Z

OTHERS	= ${FONT_LIST}

ILIST 	= ${OTHERS}
IDIR	= /usr/lpp/X11/lib/X11/fonts/misc/

.include <${RULES_MK}>

${FONT_LIST:M*.pcf.Z} : $${.TARGET:.pcf.Z=.bdf}
	${RM} -f ${.TARGET} ${.TARGET:.Z=}
	${BDFTOPCF} ${.ALLSRC} >${.TARGET:.Z=}
	${COMPRESS} ${.TARGET:.Z=}
