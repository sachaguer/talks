To create an `html` file from a talk run

```bash
quarto render <file.qmd> --to revealjs --output <file.html>
```

To turn the `html` file into a pdf, run:

```bash
decktape reveal \
  --chrome-path=/snap/bin/chromium \
  --chrome-arg=--no-sandbox \
  slides.html slides.pdf
```

`--chrome-path=/snap/bin/chromium` is needed on the personal laptop but is not needed with work laptop.