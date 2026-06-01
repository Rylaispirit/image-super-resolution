# Contributing

Thank you for your interest in contributing to this community revival fork of ISR.

## Project status

This repository is a community-maintained revival fork of the original `idealo/image-super-resolution` project. The upstream project was archived after active maintenance ended. Contributions here should preserve the original license, attribution, and research references.

## Good first contributions

- Improve installation documentation.
- Reproduce and document legacy dependency issues.
- Add small tests that do not require large downloads.
- Update examples and troubleshooting notes.
- Triage issues from the original upstream repository and link relevant context.

## Development setup

```bash
python -m venv .venv
. .venv/bin/activate
python -m pip install --upgrade pip setuptools wheel
python -m pip install -e '.[tests]'
```

The original project was built around older Python/TensorFlow/Keras dependency combinations. If installation fails on the newest Python version, please open an issue with:

- Python version
- OS
- TensorFlow version
- complete error log

## Running checks

```bash
python -m compileall ISR
python -m pytest tests -q
```

Some tests may require legacy dependency versions or sample weights. The initial revival goal is to separate lightweight tests from heavy integration tests so CI can run reliably.

## Pull request guidelines

- Keep changes focused and reviewable.
- Add tests or documentation for behavior changes when possible.
- Avoid large binary files in pull requests.
- Preserve license headers and attribution.
- Explain compatibility impact for TensorFlow/Keras/NumPy/h5py changes.

## Security

If you find a security issue involving unsafe file handling, model loading, dependency vulnerabilities, or command execution, please open a minimal issue without publishing exploit details. A private disclosure process may be added as the fork matures.
