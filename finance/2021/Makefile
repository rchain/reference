# TODO: git submodule?
# https://github.com/dckc/finquick
# https://github.com/dckc/finquick/tree/rchain-finance f9332bb
FINQUICK=finquick

balance-sheet-2021-q2.json: balance-sheet-2021-q2.txt
	node finquick/brcal/src/grokBalanceSheet.js <$< >$@ || rm $@

balance-sheet-2021-q2.txt: balance-sheet-2021-q2.pdf
	pdftotext -layout $< >$@ || rm $@

