# rm-dl-annotated

Export annotated PDFs from [ReMarkable tablets](https://remarkable.com/).

I read lots of papers on my RM tablet. It's super cool to be able to scribble
notes and highlight them, but later I want to go back and review the notes and
unfortunately the interface on the actual RM sucks for that. I made this simple
utility so I could scroll through the PDFs on my laptop and see my highlights
and notes at a glance during review.

## Example

```
rm-dl-annotated.sh "/Super Cool Research Paper I Scribbled All Over"
```

Generates `./"Super Cool Research Paper (annotated).pdf"` with the scribbles on top of the original PDF.

## Dependencies:

All these things need to be on your path, and you need to have given rmapi access to your ReMarkable Cloud account:

* [rmapi](https://github.com/juruen/rmapi)
* [rM2svg](https://github.com/reHackable/maxio/blob/master/tools/rM2svg)
* rsvg-convert
* pdfunite
* pdftk
