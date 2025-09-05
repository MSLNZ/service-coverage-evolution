To generate the report:

1. Build the PDF (creates the files required by `biber`)

```console
pdflatex report.tex
```

2. Compile the bibliography

```console
biber report
```

3. Re-build the PDF (run the following command twice to update the references)

```console
pdflatex report.tex
```

The `KCDB Data.xlsx` file is used to create the images in the `figures` directory. Each Sheet corresponds to a `output\services-by-branch-all-countries\YEAR.txt` file.
