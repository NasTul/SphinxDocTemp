`pip install sphinx`


`sphinx-quickstart docs`



```

docs
├── build           
├── make.bat
├── Makefile
└── source
   ├── conf.py
   ├── index.rst
   ├── _static
   └── _templates
   
```

`sphinx-build -b html source build`


`pip install rst2pdf`

```
extensions = ['rst2pdf.pdfbuilder']
pdf_documents = [('index', u'rst2pdf', u'Sample rst2pdf doc', u'Your Name'),]

# index - master document
# rst2pdf - name of the generated pdf
# Sample rst2pdf doc - title of the pdf
# Your Name - author name in the pdf
```

`sphinx-build -b pdf doc/source doc/build`
