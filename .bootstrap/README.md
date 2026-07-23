# EnvSync bootstrap bundle

This directory contains the one-time source bundle used to populate the implementation branch when GitHub Actions is enabled.

- Bundle: `envsync.tar.gz`
- SHA-256: `36df20ea831186c15030be6520b5029fe5a365380df24db67cb80ba11f7ed0f4`
- Archive entries: 140
- Intended branch: `feat/envsync-v0.1.0`
- Pull request: #1

The base-branch workflow `.github/workflows/bootstrap-project.yml` expands this archive, generates `package-lock.json`, creates reviewable commits, pushes the source tree, and runs preliminary validation. It removes this bootstrap directory and itself from the implementation branch after expansion.

No source code or environment-variable data is uploaded anywhere other than this GitHub repository.
