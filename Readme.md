# Overview

The NWB specification language defines formal structures for describing the organization of complex data using basic
concepts, e.g., Groups, Datasets, Attributes, and Links. See the
[documentation](http://nwb-schema-language.readthedocs.io/) for more information and release notes.

The NWB specification language is used by the [Neurodata Without Borders (NWB)](https://www.nwb.org) neurophysiology
data standard and is based off of the [Hierarchical Data Modeling Framework (HDMF)](https://github.com/hdmf-dev/hdmf)
[specification language](http://hdmf-schema-language.readthedocs.io/).

## For maintainers

The NWB specification documentation is generated using [Sphinx](http://www.sphinx-doc.org/en/stable/index.html)

### Building the documentation

Install the latest version of [Sphinx](http://www.sphinx-doc.org/en/stable/index.html):
```
python -m pip install sphinx
```

To build the documentation, enter:
```
make <doctype>
```
where `<doctype>` is, e.g., `html`, `latexpdf`.

For a complete list of supported doc-types, enter:
```
make help
```

To remove previously generated documentation, enter:
```
make clean
```

### Making a release

1. Update the release notes in `source/release_notes.rst`.
2. Update the version in `source/namespace_map.yml`, `source/nwb.schema.json`, and `source/conf.py`
