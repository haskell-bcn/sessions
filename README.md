## Available sessions

  1. Meetup kickoff (12/04/2016 @ Itnig)

## Generate output files

We use `pandoc` to generate output files from markdown:

`stack setup && stack install pandoc`

To generate `slidy` html for a certain session type the following:

`pandoc -V slidy-url=slidy -s --mathjax -t slidy s{$session-number}.md -o s{$session-number}.html`
