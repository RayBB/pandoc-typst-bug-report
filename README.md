# Pandoc Bug with Typst

This repository demonstrates a bug in the way that Pandoc resolves resource paths when converting Typst documents to PDF.
Issue present with pandoc 3.7.0.2

## Reproduction

1. Clone this repository.
2. Run the pandoc conversion of your choice:
   - `pandoc main.typ -f typst -s -o main.pdf`
   - `pandoc main.typ -f typst -s -o main.docx`
   - `pandoc main.typ -f typst -s -o main.html`
3. See how it successed in typst:
   - `typst compile main.typ`


## Gallery

### Failed Output from Pandoc (docx)
![alt text](/images/fail_docx.png)

### Successful Output from Typst (pdf)
![alt text](/images/success_pdf.png)
