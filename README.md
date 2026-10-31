![Python checks](https://github.com/leakquicked/domainintel/actions/workflows/python-checks.yml/badge.svg)

# Domain Intel

Extract domain-like and IP-like strings from local text.

## Usage
```bash
python domainintel.py sample.txt
python domainintel.py sample.txt --output report.json
```

Python 3.10+, standard library only. The tool reads a local UTF-8 text file and emits JSON findings. It makes no network requests and does not modify input files.

## Rules
- `domain` — info severity heuristic.
- `ip` — review severity heuristic.

Findings are leads for human review, not proof of compromise. Use only data you own or are authorized to inspect. Do not publish personal or confidential data.

## Tests
Run `python -m unittest discover -s tests -v`.
