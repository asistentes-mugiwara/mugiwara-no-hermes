# Publishing Policy

## Default stance

**Deny by default.**

If there is doubt about whether something is safe to publish, it stays out.

## Allowed

- high-level architecture
- abstract role descriptions
- sanitized examples
- public-safe conventions
- editorial changelogs and release notes
- diagrams without sensitive operational detail

## Requires strong sanitization

- config fragments
- prompt excerpts
- workflow descriptions
- logs or screenshots
- operational examples

## Forbidden

- secrets, tokens, cookies, credentials
- `.env` contents
- real runtime identifiers
- internal topology with exploitable detail
- raw memory or session state
- production logs
- unsafe prompts or operator bypass logic

## Publication checklist

Before publishing, verify:

- no secret material
- no live operational identifiers
- no unnecessary local paths
- no sensitive topology detail
- no runtime state
- no hidden metadata in files or images
- clear public value
