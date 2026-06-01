# Community Revival Roadmap

This fork is a community revival of `idealo/image-super-resolution` (ISR). The original upstream repository was archived after active maintenance ended. The goal of this fork is to preserve the original Apache-2.0 project while making it easier to install, test, understand, and maintain on modern systems.

## Goals

- Keep the original attribution, license, and research references intact.
- Restore a working development workflow for contributors.
- Modernize packaging, tests, and documentation.
- Review compatibility with modern Python, TensorFlow/Keras, NumPy, and h5py versions.
- Make the project safer and easier to use for educational and research purposes.

## Phase 1 — Stabilization

- Add a maintained-fork notice and roadmap.
- Add a lightweight CI workflow for basic import/package checks.
- Document the current legacy dependency constraints.
- Identify tests that can run without downloading large model weights.
- Triage high-impact upstream issues that are still relevant.

## Phase 2 — Compatibility

- Audit TensorFlow/Keras API usage.
- Test supported Python versions and document known-good environments.
- Reduce strict legacy pins where safe.
- Add regression tests for model construction and prediction helpers.
- Improve handling of model weights and local cache paths.

## Phase 3 — Documentation and Examples

- Update installation instructions for modern environments.
- Add quickstart examples for prediction with sample images.
- Add contributor setup instructions.
- Refresh notebooks or provide scripts that are easier to test in CI.
- Document model architecture at a high level for new contributors.

## Phase 4 — Releases

- Publish clearly versioned community-fork releases.
- Maintain changelogs.
- Keep dependency and security reviews part of the release process.

## Non-goals

- This fork does not claim official ownership of the original upstream project.
- This fork does not remove original attribution or license notices.
- This fork is not intended to redistribute third-party model/data assets without verifying their licenses.
