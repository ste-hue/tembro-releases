# Agent instructions — Tembro release distribution

This repository is a public **distribution surface**, not the source of truth for
product code, release readiness, or customer delivery.

Before making any change, read:

- [Launch control #70](https://github.com/ste-hue/ableton-agent/issues/70) — current state, launch gates, owners, and evidence.
- [Collaborator workflow #72](https://github.com/ste-hue/ableton-agent/issues/72) — access, PR policy, and permanent stop gates.
- [GitHub collaborator quickstart](https://github.com/ste-hue/ableton-agent/blob/main/docs/COLLABORATOR-QUICKSTART.md) — the required issue → branch → PR → CI workflow.
- [Business OS #73](https://github.com/ste-hue/ableton-agent/issues/73) — the end-to-end customer, software, data, and money model.

## Release safety gate

- Draft releases and their assets are staging material. They are **not** proof of a
  production release or a valid production download; draft asset URLs may return
  404.
- Never publish, unpublish, edit, or delete a release, and never upload, replace, or
  delete an asset, without Stefano's explicit human release approval recorded in
  launch control #70.
- Never point a website, checkout, or customer delivery at a draft asset.
- Never infer the file delivered by Lemon Squeezy from this repository. Verify the
  actual customer download in Lemon Squeezy and record the evidence in #70.
- Do not commit binaries to `main`. Propose documentation or automation changes
  through a focused pull request.

Before a release can be approved, report the source repository, tag and full commit
SHA, CI run, exact filenames and SHA-256 hashes, target channel, and applicable
signature/notarization evidence. If any item is unknown, stop and leave the work as
a draft PR or draft release with one clearly named owner and next action.
