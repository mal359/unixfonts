# @(#)50	1.1  src/bos/usr/lpp/kls/fonts/misc/Makefile, bosmsg, bos411, 9428A410j 3/24/94 10:29:33
#
#   COMPONENT_NAME: cmdkr
#
#   FUNCTIONS: none
#
#   ORIGINS: 27
#
#   IBM CONFIDENTIAL -- (IBM Confidential Restricted when
#   combined with the aggregated modules for this product)
#                    SOURCE MATERIALS
#
#   (C) COPYRIGHT International Business Machines Corp. 1988,1994
#   All Rights Reserved
#   US Government Users Restricted Rights - Use, duplication or
#   disclosure restricted by GSA ADP Schedule Contract with IBM Corp.
#

FONT_LIST = \
	hanglg16.pcf.Z \
	hanglm16.pcf.Z \
	hanglm24.pcf.Z

OTHERS	= ${FONT_LIST}

ILIST	= ${OTHERS}
IDIR	= /usr/lpp/X11/lib/X11/fonts/misc/

.include <${RULES_MK}>

${FONT_LIST:M*.pcf.Z} :	$${.TARGET:.pcf.Z=.bdf}
	${RM} -f ${.TARGET} ${.TARGET:.Z=}
	${BDFTOPCF} ${.ALLSRC} >${.TARGET:.Z=}
	${COMPRESS} ${.TARGET:.Z=}
