## Copyright 2004,2019,2021 IPB, Universite de Bordeaux, INRIA & CNRS
##
## This file is part of the Scotch software package for static mapping,
## graph partitioning and sparse matrix ordering.
##
## This software is governed by the CeCILL-C license under French law
## and abiding by the rules of distribution of free software. You can
## use, modify and/or redistribute the software under the terms of the
## CeCILL-C license as circulated by CEA, CNRS and INRIA at the following
## URL: "http://www.cecill.info".
## 
## As a counterpart to the access to the source code and rights to copy,
## modify and redistribute granted by the license, users are provided
## only with a limited warranty and the software's author, the holder of
## the economic rights, and the successive licensors have only limited
## liability.
## 
## In this respect, the user's attention is drawn to the risks associated
## with loading, using, modifying and/or developing or reproducing the
## software by the user in light of its specific status of free software,
## that may mean that it is complicated to manipulate, and that also
## therefore means that it is reserved for developers and experienced
## professionals having in-depth computer knowledge. Users are therefore
## encouraged to load and test the software's suitability as regards
## their requirements in conditions enabling the security of their
## systems and/or data to be ensured and, more generally, to use and
## operate it in the same conditions as regards security.
## 
## The fact that you are presently reading this means that you have had
## knowledge of the CeCILL-C license and that you accept its terms.
##

TXT2MAN		= 	txt2man

MANPTSCOTCHFILES=	dgmap.1		\
			dgord.1		\
			dgscat.1	\
			dgtst.1

MANSCOTCHFILES	=	acpl.1		\
			amk_ccc.1	\
			amk_grf.1	\
			atst.1		\
			gbase.1		\
			gcv.1		\
			gdump.1		\
			gmap.1		\
			gmk_hy.1	\
			gmk_m2.1	\
			gmk_msh.1	\
			gmtst.1		\
			gord.1		\
			gotst.1		\
			gout.1		\
			gtst.1		\
			mcv.1		\
			mmk_m2.1	\
			mord.1		\
			mtst.1

# Project building rules.

all		:	scotch	ptscotch

scotch		:	$(MANSCOTCHFILES)

ptscotch	:	$(MANPTSCOTCHFILES)

# Clean-up and archive rules.

clean		:

realclean	:	clean
			-$(RM) $(MANPTSCOTCHFILES) $(MANSCOTCHFILES)

##
##
##

acpl.1		:	acpl.1.txt
			$(TXT2MAN) -v "Scotch user's manual" -s 1 -t acpl -Bdeco < $(<) > $(@)

amk_ccc.1	:	amk_ccc.1.txt
			$(TXT2MAN) -v "Scotch user's manual" -s 1 -t amk_ccc -Imeth < $(<) > $(@)

amk_grf.1	:	amk_grf.1.txt
			$(TXT2MAN) -v "Scotch user's manual" -s 1 -t amk_grf -Ilfile -Istrat < $(<) > $(@)

atst.1		:	atst.1.txt
			$(TXT2MAN) -v "Scotch user's manual" -s 1 -t atst < $(<) > $(@)

dgmap.1		:	dgmap.1.txt
			$(TXT2MAN) -v "PT-Scotch user's manual" -s 1 -t dgmap -Bmpirun -Iopt -Ipnum -Ipwght -Istrat -Ival -Iverb < $(<) > $(@)

dgord.1		:	dgord.1.txt
			$(TXT2MAN) -v "PT-Scotch user's manual" -s 1 -t dgord -Bmpirun -Imfile -Ipnum -Istrat -Itfile -Iverb < $(<) > $(@)

dgscat.1	:	dgscat.1.txt
			$(TXT2MAN) -v "PT-Scotch user's manual" -s 1 -t dgscat '-B%r' -Bmpirun -Ipnum < $(<) > $(@)

dgtst.1		:	dgtst.1.txt
			$(TXT2MAN) -v "PT-Scotch user's manual" -s 1 -t dgtst '-B%r' -Bmpirun -Ipnum < $(<) > $(@)

gbase.1		:	gbase.1.txt
			$(TXT2MAN) -v "Scotch user's manual" -s 1 -t gbase < $(<) > $(@)

gcv.1		:	gcv.1.txt
			$(TXT2MAN) -v "Scotch user's manual" -s 1 -t gcv -Iifmt -Inum -Iofmt < $(<) > $(@)

gdump.1		:	gdump.1.txt
			$(TXT2MAN) -v "Scotch user's manual" -s 1 -t gdump -Iprefix -Isuffix -Ibase < $(<) > $(@)

gmap.1		:	gmap.1.txt
			$(TXT2MAN) -v "Scotch user's manual" -s 1 -t gmap -Bdeco -Idim -IdimX -IdimY -IdimZ -Ihgt -In0 -In1 -Inhgt-1 -Iopt -Ipwght -Istrat -Ival -Iverb -Iw0 -Iw1 -Iwdim-1 -Iwhgt-1 < $(<) > $(@)

gmk_hy.1	:	gmk_hy.1.txt
			$(TXT2MAN) -v "Scotch user's manual" -s 1 -t gmk_hy -B gmk_ -Icfile < $(<) > $(@)

gmk_m2.1	:	gmk_m2.1.txt
			$(TXT2MAN) -v "Scotch user's manual" -s 1 -t gmk_m2 -B gmk_ -Icfile < $(<) > $(@)

gmk_msh.1	:	gmk_msh.1.txt
			$(TXT2MAN) -v "Scotch user's manual" -s 1 -t gmk_msh -Igfile -Imfile < $(<) > $(@)

gmtst.1		:	gmtst.1.txt
			$(TXT2MAN) -v "Scotch user's manual" -s 1 -t gmtst -Bcmplt -Inum < $(<) > $(@)

gord.1		:	gord.1.txt
			$(TXT2MAN) -v "Scotch user's manual" -s 1 -t gord -Imfile -Istrat -Itfile -Iverb < $(<) > $(@)

gotst.1		:	gotst.1.txt
			$(TXT2MAN) -v "Scotch user's manual" -s 1 -t gotst < $(<) > $(@)

gout.1		:	gout.1.txt
			$(TXT2MAN) -v "Scotch user's manual" -s 1 -t gout -Bivview -Igeop -Ioutp -Irat < $(<) > $(@)

gtst.1		:	gtst.1.txt
			$(TXT2MAN) -v "Scotch user's manual" -s 1 -t gtst < $(<) > $(@)

mcv.1		:	mcv.1.txt
			$(TXT2MAN) -v "Scotch user's manual" -s 1 -t mcv -Iifmt -Inum -Iofmt < $(<) > $(@)

mmk_m2.1	:	mmk_m2.1.txt
			$(TXT2MAN) -v "Scotch user's manual" -s 1 -t mmk_m2 -B mmk_ -Icfile < $(<) > $(@)

mord.1		:	mord.1.txt
			$(TXT2MAN) -v "Scotch user's manual" -s 1 -t mord -Imfile -Istrat -Itfile -Iverb < $(<) > $(@)

mtst.1		:	mtst.1.txt
			$(TXT2MAN) -v "Scotch user's manual" -s 1 -t mtst < $(<) > $(@)
