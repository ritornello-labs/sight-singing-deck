# Listing preparation — 2026-10-07

Status: prepared for review; **awaiting explicit image/copy approval**. No AnkiWeb submission or public media upload in this pass.

The complete local review hub and native capture sources are recorded in the private workspace publication queue. GIFs use actual Anki 25.09 workbench captures from disposable profiles. Similar question/answer demos hold the question for two seconds and answer for three; interactive demos allow time for actions and feedback.

Every listing includes the Ritornello banner, gallery invitation, stable support page, and the public GitHub URL where a dedicated public repository exists. Videos are absent.

## Exact proposed listings

### Sight Singing — a function-first ear & reading course

- Listing: `release/ankiweb.md`
- Copy SHA-256: `adfbd44086b90abe75b29252cea12ec6ab1115f93d0c8c7037631118f3ea8678`
- Candidate SHA-256: `f38273ab7793f2020ed4da27c9e090efa01f418ad2a7bd61b29820cd68c8703e`
- Approval: awaiting approval
- GIF `sight-singing/sing.gif`: `65a1417578dd0a48dc43ffef86736a04e2513b9b71acb441ce3781c0171ed632`
- GIF `sight-singing/rhythm.gif`: `62200eee3d2545996035246868e09ee8d7b930c96f460af69c8f84c0d9f29ca3`
- GIF `sight-singing/error.gif`: `60c52a712ad9bb61d33b52f1a70a73b2d333435fe440d85f37dcdecf64769905`

### Music Dictation - Write What You Hear

- Listing: `release/dictation-ankiweb.md`
- Copy SHA-256: `e7be0213598a0d0648d046f03161af293cba6507768bc723c476fd6855714edf`
- Candidate SHA-256: `716662809830ab9289199477267f37c08baadd3f486f28a8c2c7fed110cada1d`
- Approval: awaiting approval
- GIF `dictation/entry.gif`: `248ab53cb7fd191ba66a0285ac26b01ca6ee33f202f0c673acf18f8a20656178`

## Upload procedure

1. Record explicit approval against these exact copy and image hashes. Any subsequent visible change requires fresh review.
2. Verify the current quota and exact original share/deck name. Open only the isolated Publisher when an export/import is needed; never operate the personal profile.
3. Wait for Elvis if 1Password or account authentication requires interaction. The scheduled reminder only pings him; it never publishes automatically.
4. Publish through `anki-addon-release`; owner-verify the listing and download its delivered artifact.
5. Attach the exact submitted/delivered bytes to a tagged GitHub release, verify its digest, and update the website gallery/release links and workspace queue.

For add-ons installed directly from GitHub release files, release notes must explain that they do not auto-update; AnkiWeb installs do.

## Export repair

Anki’s native export omitted 384 Error Detection performance clips because their filenames existed only as JSON values. Each variant now includes an inert HTML audio reference inside its hidden JSON container, which Anki recognizes for export. The public generator and disposable candidate use the same correction. All 1,827 referenced Sight Singing audio files are packaged; Dictation has 806. No source audio was missing. Native Anki parsed all six variants in the demo and preserved their random-performance behavior. The 64 affected candidate notes retain their note, model, GUID and card identities. Original Publisher and personal collection were not edited.

Both Error Detection package builders explicitly compute the legacy field-based GUID after omitting only the new export-reference property. Verification against all 64 historical candidate note GUIDs passed, so future generated packages keep updating those notes in place. Candidate artifact, listing and GIF hashes are unchanged by this generator identity fix.

The native Dictation recording places six notes through the actual card pointer handlers, then reveals feedback with five matches and one intentional difference.
