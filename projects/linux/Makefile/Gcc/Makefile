########################################################################
# Copyright (c) 1988-2017 $organization$
#
# This software is provided by the author and contributors ``as is''
# and any express or implied warranties, including, but not limited to,
# the implied warranties of merchantability and fitness for a particular
# purpose are disclaimed. In no event shall the author or contributors
# be liable for any direct, indirect, incidental, special, exemplary,
# or consequential damages (including, but not limited to, procurement
# of substitute goods or services; loss of use, data, or profits; or
# business interruption) however caused and on any theory of liability,
# whether in contract, strict liability, or tort (including negligence
# or otherwise) arising in any way out of the use of this software,
# even if advised of the possibility of such damage.
#
#   File: Makefile
#
# Author: $author$
#   Date: 10/12/2017
#
# Linux Gcc Makefile for meta Makefile project
########################################################################
OS = linux
PFX =
FWX = ../../../../..
PKG = ../../../..

MAK = projects/Makefile/Gcc
PRJ = $(PFX)projects/$(OS)/Makefile/Gcc

include $(PKG)/$(MAK)/Makedefines

rt = $(FWX)/nadir/$(PRJ)/lib/librt
nadir = $(FWX)/nadir/$(PRJ)
coral = $(FWX)/coral/$(PRJ)
medusa = $(FWX)/medusa/$(PRJ)
talas = $(FWX)/talas/$(PRJ)
evelation = $(FWX)/evelation/$(PRJ)
evup = $(FWX)/evup/$(PRJ)
xde = $(FWX)/xde/c/projects/$(OS)/gcc
medusaxde = $(FWX)/medusaxde/c/projects/$(OS)/Makefile

#
# Source subdirs
#
#SRC_DIRS = \
#$(PKG)/$(PRJ)/somedir \
#
ifndef SRC_DIR
SRC_DIRS = \
$(nadir) \
$(coral) \
$(medusa) \
$(talas) \
$(evelation)
else
SRC_DIRS = $(SRC_DIR)
endif

include $(PKG)/$(MAK)/Makedirs

rt:
	@(make SRC_DIR=$(rt) $(target))

nadir:
	@(make SRC_DIR=$(nadir) $(target))

coral:
	@(make SRC_DIR=$(coral) $(target))

medusa:
	@(make SRC_DIR=$(medusa) $(target))

talas:
	@(make SRC_DIR=$(talas) $(target))

evelation:
	@(make SRC_DIR=$(evelation) $(target))

evup:
	@(make SRC_DIR=$(evup) $(target))

xde:
	@(make SRC_DIR=$(xde) $(target))

medusaxde:
	@(make SRC_DIR=$(medusaxde) $(target))

