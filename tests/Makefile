ROOT = ..
include ${ROOT}/defs.mk


diff = diff -u

ensemblGff3ToBigEnsembl = ${BINDIR}/ensemblGff3ToBigEnsembl

test: chm13Test hprcTest

chm13Test: mkdirs
	${ensemblGff3ToBigEnsembl} input/ensembl.chm13.gff3 output/$@.gp

hprcTest: mkdirs
	${ensemblGff3ToBigEnsembl} input/GCA_018466835.1.gff3 output/$@.gp


mkdirs:
	@mkdir -p output

clean:
	rm -rf output
