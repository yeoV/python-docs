# Sphinx
- Sphinx is a documentation generator
- reStructuredText or Markdown documents to HTML, PDF,,, etx

## Installing

### Linux
- Debian/Ubuntu
``` bash
$ apt-get install python3-sphinx
```

### macOS
``` bash
$ brew install sphinx-doc
```

### Anaconda
``` bash
$ conda install sphinx
```

### PyPI
``` bash
$ pip install -U sphinx
```

### source
```
$ pip install git+https://github.com/sphinx-doc/sphinx
```

### Checking install
```
$ sphinx-build --version
```
***

# Getting Started
- create documentation layout
```
$ sphinx-quickstart docs
```
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



## Setting Markdown file
```
$ conda install -c conda-forge myst-parser    # conda
$ pip3 install myst_parser     # pip
```
- config.py
```
extensions = ['myst_parser']
source_suffix = {
    '.rst': 'restructuredtext',
    '.txt': 'markdown',
    '.md': 'markdown',
}
```


## RTD Theme
- install
```
$ conda install sphinx_rtd_theme
```
- config.py
``` python
html_theme = 'sphinx_rtd_theme'
```


## Build
- Makefile builder
```
$ make builder
```
- 소스파일 / build 파일 따로 분리한 경우
- .rst 파일을 생성해준 후 build
```
$ sphinx-apidoc -f -o docs/source <dir>
```


## reStructedText docs
- https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html