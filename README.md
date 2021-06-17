# My IEEE Template
This repo contains a basic IEEE Transactions template set. Please note that this
is *NOT* the official IEEE template, and is purely a structural organization of
how I use the template when I write papers.



## Organization
"special" sections are noted here. 

* `paper.tex`: top level document containing `\input` and `\include` to your
	paper.
* `sections/000-draft_files.tex`: controls and flags for disabling authors,
	draft mode, or text coloring.
* `sections/000-extrapackages-ieee.tex`: default IEEE suggested packages.
	Comment/uncomment them as documented inside by Dr. Shell.
* `sections/000-extrapackages-local.tex`: any modifications you want to make
	(before `\begin`)
* `sections/001-head_material.tex`: abstract and index terms
* `sections/099-todostuff.tex`: list of *todo* items generated in the paper


## Useful commands

* `\todo{<msg>}`: provides markup in the margins
* `\hlfix{<text>}{<msg>}`: highlights `<text>` in the body, and pairs it with a 
	`\todo`
* `\editB{<text>}`: changes text color of `<text>`.
	* `\editR`, `\editG`, `\editBB`, `\editRR` also provide 4 extra colors. Red, 
		green, not-blue, and not-red.
* `\dummy`: a citation to `FooBar` as a filler. It also inserts a `\todo` to
	make sure you actually go back and fix the dummy citation later.
	* `\dummy[<msg>]` will replace the default text in `\todo` with `<msg>`

## Upstream Template
The upstream is maintained at:

* [http://www.michaelshell.org/tex/ieeetran/](http://www.michaelshell.org/tex/ieeetran/)
* [http://www.ctan.org/pkg/ieeetran](http://www.ctan.org/pkg/ieeetran)

---
