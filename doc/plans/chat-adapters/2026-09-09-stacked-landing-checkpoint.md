# Chat implementation landing checkpoint — September 9, 2026

This working note can be deleted after both landing PRs merge and the remaining
live hardening is represented by its own follow-up PR.

## Durable snapshot

- Snapshot revision: `007399bcd207f33aee7b62d14cf7a854cb979eca`.
- Snapshot tree: `5ba0226bedf205102b01ab7fae5d8bdf98cb832f`.
- Immutable local recovery branch: `codex/chat-adapters-snapshot-20260909`.
- Parent: `9afdf3232d2ac781ce4af05350129a6a8c7e2eb2`.
- Captured all 29 modified/new implementation and qualification-document paths
  using an alternate Git index. All 29 working-file hashes matched the snapshot.
  The original checkout's HEAD and empty staging area were unchanged.
- Landing worktree: `/Users/dotta/paperclipai/branches/chat-adapters-landing-20260909`.
- Initial landing branch: `codex/chat-adapters-landing-20260909`.
- Origin master at snapshot: `5acf56658bff7eeb12438a6fdcae5f4d2fe1e90e`.
- Ignored live runtime, credentials, databases, generated packages, and the
  protected runner binary were not added. Changed/new files passed the scoped
  credential-marker scan. This is not a claim of a full repository secret audit.

## Separate lanes

The user explicitly authorized the separate landing worktree and superseded the
earlier no-new-worktree/no-PR-tending constraints for this lane. James owns
reconciliation, exactly two coherent stacked PRs under 500 changed files each,
fresh exact-head Greptile 5/5, required checks, and dependency-ordered merges.
The existing PR is https://github.com/paperclipai/paperclip/pull/13038; it had 526
changed files and conflicts at this checkpoint. Preserve its review context
where practical. Do not merge based on old review scores or narrow local tests.

James exclusively owns remote `codex/chat-adapters` updates while reorganizing
that PR. The original local branch must not push over the landing heads. Do not
modify the original checkout or live runtime from the landing worktree.

The root, Epicurus, and Boole continue live stress qualification and subsequent
hardening in the original checkout. Changes after the snapshot remain separate.
After both merges, reconcile the ongoing branch with merged master, preserve
newer fixes, and open a follow-up PR without reintroducing landed changes.

## Verification boundary

Snapshot evidence: Board attachment cohort 417/417; blocked-continuation cohort
36/36; Rust durable-runner cohort 36/36; plain server/UI/runner TypeScript checks
passed; token gates clean. The full transport cohort was still running. These
are focused checks, not current-head full repository or landing CI verification.

Server 78 remained running on port 3137. Its loaded version was
`2026.831.0+623.git.ea528f44c`; a dynamically read Git HEAD is not proof that newer
source was deployed. No live restart or protected binary replacement occurred
while creating the snapshot. Historical quarantined recovery evidence remains
untouched.

## Subsequent checkpoint — 13:52 UTC

Base PR [#13092](https://github.com/paperclipai/paperclip/pull/13092) is open
with 45 changed files. Master reconciliation has exposed additional native
goal/integrity and PRP-v2 warm-authorization/state-retention defects. James owns
their landing-only regressions; neither the initial PR head nor historical
Greptile reviews certify the corrected head. The current-master warm-upgrade
compatibility boundary must be explicit, not hidden by a fail-closed test.

Root's test-only `5232fb22b` is available for the second PR. The new Board
uncertain-write and late-semantic-result hardening remain post-snapshot work.
A newly observed live Discord close/recovery loop must be fixed and qualified
before the experimental connector PR merges; it is not cosmetic follow-up.
Maya is temporarily paused to contain that loop. No deployment occurred.

## Subsequent checkpoint — 14:02 UTC

The base is now 47 files at `3e7289cd4` (James owns publication and exact-head
checks). Its prior head's Greptile 5/5 does not certify this head. Full workspace
build passed in the isolated landing worktree; full tests/checks remain pending.
The post-snapshot semantic-result fix is included in the base via its exact
four-file delta, not a duplicate cherry-pick of the full snapshot-containing
commit. Root's local commits are `c76988f93` (runner) and `ae21fd9e2` (Board).

The real process-replacement test proves a **v2-capable current artifact** first
leased as v1 can retire its exact owner and negotiate v2 on fresh bootstrap,
preserving native cached state before a warm attach. It does not prove an old
binary upgrade: the existing restart closure retains its original artifact.
Same-lease reconnect remains v1; adopted owners have no automatic upgrade path.
Do not advertise this internal recovery proof as a new operator upgrade API.

Board qualification finished 350 focused units and 11 actual browser journeys.
Runner release qualification finished 27 composed tests, in addition to 227
serial source tests. The close/recovery defect has two clean failing regressions
and remains a merge gate for the top PR. All live runs remain deliberately
paused. The original live binary and lockfile are unchanged.

## Subsequent checkpoint — 14:35 UTC

The current published base is `46ef7ef03ca35a47d6ac2be9e2dd497b137d3b70`,
44 changed files. Its exact-head Greptile score is 3/5; the prior 5/5 scores
do not satisfy the merge gate. James is addressing the concrete review
findings and current-master compatibility fixtures in the landing worktree.
The full runner suite at that head was 1,881 passed, six failed, ten skipped;
focused corrected fixtures do not replace the required fresh full-suite run.
Master has advanced through `35fdc0c66`, including durable task recovery work
that the top PR must preserve rather than overwrite with the older snapshot.

The original checkout's full chat integration suite is now **860/860 passed**
on fresh database `chat_snapshot_full_20260909_root06`, through test/copy fixes
in `02dc80d1e`. This is not a landing exact-head or full-workspace result.
All earlier failed runs remain recorded in the qualification notes.

The last close/recovery crash window has a genuine failing regression:
restoring the old blanket native-recovery exemption dispatches one provider
attempt after a committed close, where zero are allowed. The replacement
records exact-run `required`/`admitted` admission evidence in the server-owned
runner profile and preserves historical, already-admitted recovery behavior.
Nine focused cases pass; the final full recovery suite and final review are
still pending. These tests compose real native preparation and the actual
restart classifier, not an operating-system process crash.

Server 78 remains unchanged and Maya remains paused. The qualified release
runner has been copied to a private, read-only QA path but has not been
activated. A fresh database backup and controlled cutover precede the next
live question/form/close and attachment-fallback qualification.

## Subsequent checkpoint — 15:18 UTC

Base `335b2ee52709afb3885d4d6ebb2a3ece4b5864d6`, 47 changed files,
received a fresh Greptile **5/5**, clean security review and fully successful CI
run `34367194680`. Its complete local runner suite passed **1,888 tests**, with
10 preexisting skips. The whole release Rust workspace passed with serial test
scheduling and unchanged deadlines. A default-parallel attempt still exceeded
the descendant-lineage fixture's five-second deadline under load and remains
recorded; it was not hidden by the isolated or serial pass.

Master subsequently advanced to `82f662656` (#13093–13095, #13097). The base
now has a runner-transport merge conflict. The landing agent will finish
collecting its running broad 335 test result before changing source, then
reconcile and requalify the new head. The 335 approvals/checks do not authorize
merging a later head without fresh verification.

Top reconciliation must preserve master's execution recovery ordering and the
snapshot's physical-owner/usage fences. In particular, a Board reconciliation
on a chat-bound task cannot create both a generic pending successor and a
separate authorized failed-chat retry. The proposed typed single-owner receipt
keeps current chat source/access checks and existing idempotent retry identity;
non-chat behavior stays unchanged. Joined regression evidence is required.

Root deployed server 79 from local `3f2387073` and resumed Maya. Discord's
native question/choice/free-text flow passed live; Slack's true queue and native
Stop/fresh-follow-up passed. Fresh Discord close exposed an old-definition
registration incompatibility; GitHub's private-file Board fallback exposed an
unwanted passive-wait continuation and a misleading already-bound-file send
error. Repairs and final tests are in progress in the original checkout and
have not been pushed over the landing branch. Exactly two coherent PRs under
500 files and dependency-order landing remain the required structure.
