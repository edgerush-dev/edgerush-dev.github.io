# edgerush-dev.github.io

The website at [edgerush.dev](https://edgerush.dev): static HTML pages, with no
build step, no scripts and nothing loaded from elsewhere. The project itself lives in
[edgerush](https://github.com/edgerush-dev/edgerush).

GitHub Pages serves the `main` branch as it is. `CNAME` names the domain, and `.nojekyll`
stops Pages from running Jekyll over the files. To preview a change, open `index.html` in a
browser.

`index.html` describes the project goals, current feature set and implemented proxy
architecture. Keep ambitions distinct from working features; rate limiting is still in
progress, and its architecture is not ready for publication. The proxy overview is grounded
in `crates/proxy`, `crates/config`, `crates/router` and `crates/explain` in the code repository,
and the parent workspace's `docs/03-data-plane.md` and protocol docs. Check implementation
as well as design docs before expanding it. Preserve the script-free, self-contained style.

`benchmark-2026-10-04.html` is a dated
development snapshot, with methodology and limitations beside the results. Keep the
ordinary and PGO builds separate, retain unfavorable results and error counts, and do not
carry these numbers forward as measurements of later features. The source summary is
`benchmark-2026-10-04.md` in the parent workspace; the published page explicitly records
the measurement scope and links to the harness at the measured revision.
