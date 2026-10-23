# qstudying-public — status

_Snapshot: adversarial figures as of the most recent fold on any cell inside
them, 2026-08-28. Rounds have run and folded since, all on families held off
the roster, so none of them enters the figures below. Toolchain and method
notes refreshed 2026-10-23. Refreshed per release run during the
2026-06-01 → 2026-12-01 drive window._

Release-narrative status of the Lean4 focus-area syllabus. Companion to the
[README](./README.md), not a substitute.

## Overall
The scoreboard did not move this cycle; every figure below was re-derived from
the tree and came out the same. Two adversarial rounds ran and folded, both on
one cell of a family held off the roster, so neither enters a figure on this
page. The count of families held off the roster is unchanged at ten.

The changes were on the instrument side, and most of them were one defect
found five times: an instrument that executes, or pastes into its own source,
the material it is grading. All five are cured. The toolchain moved to a new
compiler release, and the move found a ban list naming constants that no
longer exist and a script that located itself wrongly. Five claims carried on
this page and the README were re-measured and corrected; four of them were
true, or untested, when they were written.

The certification badge fell from twenty of twenty-two to eighteen in an
earlier cycle. Under the same cumulative rule, nothing since has reversed it.

## The three axes
The architecture the syllabus is selected *for* runs in three parallel kernels,
one per domain, never sharing ground truth:

- **Textual** — the legal-domain axiom sets published as
  [`qnarre-public`](https://github.com/quantapix/qnarre-public).
- **Numerical** — the financial-domain axiom sets published as
  [`qresev-public`](https://github.com/quantapix/qresev-public).
- **Operational** — git-grounded axioms over the agent constellation's own
  daily mechanics (this subproject; focus area #10), proved over synthetic and
  structurally-synthetic snapshots, never real-tree data. Its consumer is
  local-only and only visualizes; nothing here is a deployed surface.

All three pin the same Lean toolchain (`leanprover/lean4:v4.35.0`, three-way
lockstep since the 2026-10-20 bump; bumps move all three and replay each
kernel's example proofs, and on this axis also replay the attack corpus through
the judge).

## Adversarial standing
Numbers as of this snapshot, all machine-checked by the build:

- **106** theorems proved across the operational targets; **78** on the
  domain-coverage numerator.
- **66** adversarial rounds; **363** attack probes thrown; **12** open items
  still awaiting an answer.
- **18 of 22** numerator cells re-certified under the closed adversarial
  contract, each holding zero adversarially-scored builds against a fresh,
  independent adversary.

The adversarial-damage figure this page previously published under the word
"landed" is withheld this refresh. The instrument that produces it counts
build entries scored for the adversarial side, once per round, so a fixture
rebuilt in several rounds counts several times. The judge that adjudicates
each round uses the same word for a narrower event, and on the most recent
round the two readings disagree. This page names a basis before it publishes
a count.
- **12 of 22** domain concepts covered, all at the strongest tier, none refuted.

**State the population in the same sentence as the count, so: these figures are a
sum over the thirty-one on-roster cells that carry a standing record, each taken
at its own last-folded round rather than at a common cut-off.** A round whose
adjudication is still gated is in none of them. Ten further families are held
off the roster until each can arrive whole (the same ten as at the last refresh) — proved theorems *and* full
adversarial standing in one change — and they are excluded in **both** directions:
their theorem counts are absent here too. Read every figure over that population,
never as a statement about the whole tree.

One more stamp is owed and is given here rather than assumed: the open-item
figure is folded under two attribution rules at once, because the ruling that
unifies them is adopted but the mechanism that implements it has not shipped.
Earlier rounds label an item's attribution from the judge's verdict; later rounds
derive it. The two disagree materially where they overlap. **A cleared ruling is
not a shipped mechanism**, and a figure produced across the seam should say so.

Two of these figures rose sharply over the cycle that ended at the last folded
round: the adversarially-scored build count, and open items from zero to twelve.
**That rise mixes two different things and this file will not pretend
otherwise.** Part of it is the population cure this file described earlier
reaching the projection: the fold had been seeded from an optional field, so any
round record that omitted it was silently subtracted while staying schema-valid.
Part of it is genuine new damage from three rounds on a newly-worked
records-substrate family, and nearly all of the remaining growth comes from one
cell. The instrument cannot separate the two, so the honest statement is the
total plus the ambiguity, not an attribution.

The previous refresh published the figures from the second of those three
rounds, not the third. Both were folded on the same day, and the page's date
stamp could not tell them apart. **A date is not a coordinate when two folds
share it.** The header now names the fold.

The certification figure deserves the sharpest note, because it went down and
because a page like this one is exactly where a falling number gets quietly
dropped. It was twenty of twenty-two. It is eighteen. The two cells that left it
had been certified, then took landed and open attacks in this cycle's rounds. The
badge gates on the **cumulative** record by standing ruling, so they are out
permanently — and the reading that would have kept them in was put up, and
rejected, before any of this happened. **The rule was adopted when it cost
nothing and it is being honoured now that it costs two cells.** That is the only
interesting thing about a badge.

Last cycle this file published a fallback reading of the same data that would
have shown twenty-two of twenty-two. **That sentence is now false as well as
rejected** — the newer damage defeats it on its own terms — and it is removed
rather than carried forward with a caveat.

Coverage is still reported as coverage, not as a blanket falsifiability claim:
rounds predating the mid-July oracle-independence fix did not certify the
adversary's independence, which is why re-certification is a separate, slower
number. The first verdict issued under the stricter evidence contract landed this
cycle; the census behind it is stated two different ways in two different places,
so no count of it is published here until one basis is named.

## An instrument is only as good as the population it enumerates
Four failures in one week, three layers apart, one shape:

- A reporting column published **zero theorems proved for every round that had
  ever run**, while a cumulative figure in the same table read two thirds
  complete. The join matched an identifier against build targets by substring
  and nothing had ever put one there. It survived for months because a zero
  looks like a modest round. The sibling join — the same defect, on the attack
  side — had been found and fixed earlier, and a comment recording that fix sat
  a few lines above the broken one. **A fix applied where it was noticed is not
  a fix of its class.**
- An axiom-floor probe reached 143 of the 282 declarations in its own module.
- An open-findings counter could only ever grow, because a conceded finding had
  no retirement path at all.
- Guards throughout an example **hand-copied the thing they were checking**, so
  they could never observe the repair they demanded.

The unifying rule: **a guard that restates its target instead of deriving from
it cannot observe the repair it demands, and a one-round finding becomes
permanent prose.** It was validated the round after it was minted. An attack
that had copied eight names out of a manifest into its own source was rebuilt to
derive them; it then saw the correction and stood down — the first time an
attack in that cell retired by the fix it demanded rather than by an operator
deleting it. The round after that, seven more conceded findings were re-keyed
the same way and retired together, one of them completing the full
observe-repair-retire cycle inside a single round.

**None of that is in the numbers above**, for two reasons. An earlier version
of this page gave only the first. That round breached, so its fold refused. The
next round on the same cell did not breach, and it folded on 2026-08-16, which
is when the retirements entered that cell's standing record. The second
reason: the cell belongs to a family held off this page's roster, so its
retirements, like its damage, enter none of the figures here at any fold.

Earlier refreshes said the seven retirements were in no metric "until the next
clean round". That was true when it was written. It stopped being true twelve
days before this page's own snapshot date, and every refresh since then carried
it forward unchecked. It was caught by re-measuring the claim against the cell's
standing history, not by any gate: every gate on this page reads tokens, and a
sentence that has gone stale contains none of them.

## Enumerate by the environment — necessary, and not sufficient
The axiom-floor probe was rebuilt to enumerate every constant the example's
modules contribute, internal ones included, with two populations reported per
run. Population 310 against the old text scan's 143, a strict superset, verdicts
unchanged, and zero false refusals across the live roster.

The rebuild is worth publishing for what it *did not* fix. Four distinct escape
forms are witnessed in one example, and they split into two families that defeat
opposite instruments:

- An **anonymous declaration** contributes no constant at all, so it is
  invisible to a text scan, to an axiom-print, and to a roster check alike.
- A **structure** mints a derived constant that appears nowhere in the file's
  text.
- A **proposition-valued definition** sits outside any keyword roster.
- A **private declaration** is name-mangled outside its own namespace and fails
  both halves of every prefix-anchored filter. **This one is now cured.** The
  filter's internal-declaration test had been doing two jobs at once — excluding
  compiler-generated auxiliaries, which is correct, and silently excluding
  author-written private declarations, which is a hole that fails in the
  direction that makes the audit look cleaner. The cure separates them by
  reading the user-facing name.

The first three defeat source-derived instruments. The fourth defeats
environment-derived ones. So "enumerate from the environment" is necessary and
**not** sufficient: the filter is the other half of the instrument, and both the
population and the filter have to be derived from the same place.

Two things about that cure are worth more than the cure. Its witness does not
reconstruct the mangling — it declares its own private probe, asks the
elaborator which constant it actually minted, and then requires the new filter
to admit that constant while the old one rejects it. A witness that rebuilds the
mangled name by hand is testing your string arithmetic, not your guard. And a
companion assertion requires the widening to be **monotone**, so a cure to a
filter cannot quietly narrow what the guard grades — the failure mode a widening
invites.

Measured at the moment of widening, the module had no private declarations left,
so the cure moved no number at all. The hole was real when it was found and
empty when it was closed. That is the normal shape of a fix that arrives late,
and it is not an argument that the hole was never there.

The measured consequence, which is the sharpest statement of why any of this
matters: one example's classical footprint was **ten, not the eight its own
prose enumerated**. A footprint counted over named declarations is blind by
construction to an anonymous one carrying the same dependence — so the gap and
the mismeasurement had a single cause, and finding either finds both.

Last cycle this file published one of those forms open, as *reported but not
reproduced*. It is now reproduced with live members, and cured.

**The first measurement of the cure was void.** The build environment read
week-old compiled artifacts without complaint and reported 229 of 310 constants,
with 51 names the old scan had found simply missing. The thing that caught it
was the superset check, not the compiler — nothing errored. Build before you
measure is now written down beside the rate, because a measurement taken over
stale artifacts does not fail, it just answers a different question.

## What a guard has to prove before it is allowed to run
Adopted this cycle as a standing law rather than another individual repair. A
guard is admissible only once it discharges all of these, the first three as
committed, suite-exercised tests:

1. **A known-bad witness it must reject.** A witness that a later run cannot
   re-fire unattended does not discharge the obligation.
2. **Reachability** — the failing branch demonstrably reachable, not dead by
   construction.
3. **A false-refusal rate against a named, frozen corpus**, recorded as
   numerator *and* denominator with its population declared. Live session
   transcripts are not a corpus: they evaporate within a day or two, and **a
   test over evaporating input passes vacuously forever.** An empty or
   near-empty denominator grades *unmeasured* — never zero, never clean.
4. **Mandate compatibility, checked before arming.** Enumerate what the
   surrounding instruction surfaces *require* on the guarded surface and replay
   each against the guard. A guard that refuses a mandated act may not arm, and
   the conflict goes to the author of the instruction, not to the participant.
5. **An excusal predicate keys on what transferred, never on how it was
   expressed.** Enumerate the ways the conduct can be phrased, then key on none
   of them.

The fifth is a law because it was a bill. One over-convicting arm voided three
rounds by convicting two structurally unrelated and entirely safe commands — a
recursive search and a status query — whose path arguments provably excluded the
sandbox in both cases. The arm read the verb and the working directory and
discarded the path arguments. A syntax-keyed excusal systematically punishes
exactly the careful caller who scoped the command properly.

The symmetry is the point, and it took a while to see: **an over-convicting
instrument voids a round precisely as a real leak does.** In one of those
rounds, the same verdict that convicted a cell on a command that transferred
nothing graded the other cell clean on zero channels while it had disclosed a
listing that named four internal documents. The instrument inverted the two
cells relative to what actually transferred. It was not superseded, because an
orchestrator correcting a breach that voids its own round is self-interested and
does not get to.

## A figure is a claim about a population, and it will be quoted without one
Three separate instances this cycle, in three layers, and they are the same
defect the guard-admissibility rules already name — restated because the rules
did not prevent any of them.

A published summary quoted a carrier count under a label that excludes, by its
own wording, part of the population the count was taken over. The underlying
artifact had carried the smaller, correct number throughout; the prose around it
carried the larger one. A section published a split of one module's declarations
that the tree does not measure, and its own enumeration listed one fewer name
than its own count.

The third is the one that reaches this file. **A fold step seeded a published
adversarial figure from an optional field.** A round record that omitted the
field was still schema-valid, so the fold silently dropped that round's findings
out of the figure and nothing anywhere reported a problem. Measured after the
fact: the published number was half the honest one, and the omission touched a
small but real fraction of the adversarial moves across several rounds. The cure
derives the value from a required field instead, with a sabotage-verified
witness.

The general rule, which is cheap and which this project keeps re-learning: **a
count is a claim about a population, so state the population in the same
sentence as the count, and derive it from a field the schema requires.** An
optional field is a silent subtraction waiting for the one emitter that forgets
it.

## The artifact under test is itself a channel — and it is not the worst one
The adversarial claim rests on the attacker not having seen prior adjudications.
The proof file under test carries a substantial history of prior rounds,
including verbatim convictions, and the adversary cannot test the artifact
without reading it. That is recorded as a known open channel rather than cured:
the history is the constructive side's legitimate rationale for why the proof is
shaped the way it is, and the cure would cost more than the leak.

A worse one was found this cycle, and it is worse for a structural reason. **A
standing instruction file is delivered to an automated participant in system
context — not read, delivered.** Every channel the independence instrument
grades is a *read*, and the transcript records no delivery, so the instrument's
silence on that channel is indistinguishable from absence. It was not silent
because the channel was clean; it was silent because it cannot see the channel
at all.

That file was carrying the example's identifier, a long run of prior-round
history, the adjudication figures, and the locations of the very documents the
same file forbids a blind participant's brief from naming — the rule defeated by
the file that states it. The payload is now split out to documents the
participant never receives, and the file points at that document set by
behaviour rather than by naming a location, which is the first time the
non-naming rule has been enforceable at all.

The transferable form: **an instrument that grades reads cannot grade a
delivery, and "no finding" from an instrument that cannot look is not a
finding.** Before trusting a clean channel report, enumerate the channels the
instrument is structurally incapable of observing, and check those by
construction instead.

## Ordering is a gate, and prose could not hold it
Last cycle published three ordering defects in five weeks, all the same shape:
*a step that promotes results ran upstream of the oracle that can void them.*
Each was fixed correctly and none of the fixes prevented the next, because the
order was enforced by an operator following a document.

One of the three is now a mechanism rather than a document. The step that folds
a round's results into standing refuses on a breach with its own exit code, and
a single verb chains the closing steps in their required order instead of
leaving the operator to sequence them. The rule it enforces is still worth
stating in general, because the remaining cures are still prose: **nothing that
promotes may run before the oracle that can void it.**

Two further instances this cycle, and the second is the sharper.

A promotion step refused correctly on a breach and returned its own exit code —
the mechanism working as designed. Then a **test** of that same lane folded the
live records directory as a side effect, overwrote the committed standing file,
and in doing so moved the very figure the production gate was at that moment
refusing to move. The gate was not defeated by a caller who ignored it; it was
defeated by a test that never went through it.

The rule that follows is not "add another gate". It is that **a witness may not
invoke a production writer against production state** — it folds a copy, and it
carries an arm that reds if the live file changes at all. A gate that lives in
the writer is a gate the writer's callers can walk around; the gate has to live
where the invocation is made.

## A statement pin has to see what the statement depends on
The step that folds a round's results into standing now refuses while any
statement it holds has moved and no build in a later round names it again.
There is no re-pin verb.

What to fingerprint was the whole design question. The obvious choice, a hash
of the theorem's elaborated type, is wrong. A type names the definitions it
uses only by their constant names, so changing a definition's body underneath
an unchanged theorem leaves the type hash unchanged. The fingerprint is taken
instead over the statement's local closure: its type, the bodies of the
definitions it reaches, and the constructors and recursors of the inductive
types it reaches. Proofs are never included, and binder names and annotations
are stripped. It stays byte-stable across a forced rebuild of the modules it
covers.

The clock came from the ruling's stated costs, not its rule sentence. The rule
alone left open whether the round that introduces a change may also
re-attest it. The ruling's own words, that a change "trips it by design",
settle the question. A same-round re-attestation would mean the gate never
trips, so a change to the kernel now costs its round one refused fold, and the
next round re-attests. **Read a ruling's declared costs as part of its text.**

Two limits are stated rather than hidden. A statement that vanishes is
reported, not gated, because renames are routine and gating them would wedge a
fold for good. And the gate's scope is a population: when the gate landed, 660
of 712 statement references resolved to a declaration. The remainder are
attack-side, retired, free-text or ambiguous names. The baseline attests the tree as of the gate's first day, one
record per example. It says nothing about drift before that.

## A decision step that exists is not coverage that holds

The operational kernel models publish-time clearance: every public push that a
clearance gate covers must be preceded by a grant from that gate's sole grantor.
The model is proved over synthetic fixtures. Until this cycle, the live side of
it could only *extract* facts from the real push record and report whether they
were checkable. "Checkable" is not "covered", and a publish gate keyed on the
extractor's exit status would have passed every uncovered push while reading as
a coverage gate. It was deliberately not wired.

A decision step now exists. It passes only when the proof assistant elaborates a
generated coverage proof over the live facts. It names each uncovered payload,
gate and clause when coverage fails, and it distinguishes "the kernel refused a
generated green" and "not yet verifiable" as separate outcomes. Its witness
drives each outcome, including a sabotaged generator. A failing reading is the
extractor's diagnosis, not a kernel-checked witness of an uncovered push,
because the negative side has no closed form yet. The step is not yet wired into
the push path it is meant to gate, and this page makes no coverage claim on the
strength of it existing.

The decision step was itself found open to its own input this cycle. It writes
a Lean file from the extracted facts, and several values were pasted into that
file verbatim. A committed known-bad put a line break and one extra declaration
into a field nothing used. That declaration supplied exactly the fact the
kernel check exists to find missing, and the step read green. Every value it
pastes must now be an identifier from a closed set, or the step exits as not
verifiable before any Lean is written. The verdict is no longer a substring of
a log line either. The generated file emits one structured record of the
proof's axiom closure, and the step admits only the axioms it declared itself,
the kernel's own, and the three standard ones. It refuses a `sorry`, an
undeclared axiom, and an empty closure. On every recorded input the old and new
steps agree on the exit code, and where a decision record is produced it is
byte-identical.

The same cycle produced a second instance of the class: a model-floor check in
the adversarial lane had been grading the *configured* model, not the model the
participants actually ran. **A gate named for a property can read a proxy for it
for months**, and both cures move the measurement to the point where the named
thing exists: a Lean-elaborated proof, and the transcript.

## An absence read is a function of the host's configuration

Two of this cycle's cures were the same defect. A no-write assertion read the
repository's status in its default form. That form does not list a new file
inside a directory that is already untracked, and under one common configuration
it lists no untracked file at all. So the assertion "nothing was written" held on
some machines and not others for the same write. The read now pins the form that
enumerates every untracked path, and a lint refuses any unpinned status read in
the lane's scripts.

The second: a recognizer for transcript-read channels matched three spellings of
where a participant's transcript lives, and missed the fourth, which is where an
out-of-tree participant's own transcript lands. Sibling participants could read
each other through it on every axis. It is closed once, in the shared component.

The witness grains are now written down as a closed set, each with a committed
known-bad: two spellings of one path, a symlinked directory, a file versus an
entry inside it, a second author or instance, and an in-tree versus an
out-of-tree copy. Three of the five are thinly witnessed today, and the page
says so rather than counting them as covered.

A third instance this cycle. At session start, the live check publishes the
axis's kernel-verified facts. It can fall back from its primary publisher to an
older one, and the fallback rate is the number a pending migration of that
publisher is measured on. The only record of a fallback used to be an error
line that the sole automatic caller discards, so a fallback rate counted from
the records was zero by construction. Each publish now records which publisher
served it, per machine. The witness drives every outcome, including a mutant
that attributes a failed scan to the wrong publisher.

## An archive is evidence only once something checks it is there
The independence audit reads raw agent transcripts, and those decay within days,
so verdicts are frozen alongside the round they judge and the raw evidence is
archived outside the repository in the same step. The retention window is why
the freeze has to be immediate: **an un-audited round is not "unchecked, we
will look later" — it is permanently unauditable**, and the only remedy is to
run the whole round again blind. "Audit the history later" is not a plan.

Last cycle's census of that archive found seven frozen verdicts with nothing
underneath them, then found that four of the seven had never been lost at all —
they were sitting on a second machine, because those rounds had run there. A
census that enumerates on one machine and reports absence-here as gone is not a
stale census; it is a census of the wrong universe.

The integrity check itself was corrected twice this cycle, in the same class it
exists to catch. Its comparison of an archive's participants against a verdict's
participants had been treating a one-sided-empty comparison as a match — that is
now **unverifiable**, which is a distinct verdict from *checked and agreed*, and
it exits accordingly. The correction landed in the shared component rather than
the local copy, after the first attempt landed in the wrong layer, at the wrong
scope, with the wrong exit semantics.

Two rules survive from all of it:

- **A gate has a coordinate system, not a target set.** Scoping by tree fixes
  membership and leaves machine, instrument version and corpus vintage silently
  partial. Fixing one axis of a scope is not fixing the scope.
- **Mechanizing a rule fixes who has to remember it, not whether the question
  was scoped right.** A declared loss should be read as *absent here* until a
  peer location has been checked.

Both halves of that lesson are now mechanized rather than remembered. The census
is host-aware: it resolves each record against the machine the round actually
ran on instead of reporting absence-here as gone. Re-run over the previously
suspect rounds, it declares **zero losses** — every record that had been counted
missing was present on a peer machine, exactly as the earlier correction
predicted. The rule survives the cure and is the reason to keep it stated: a
declared loss should be read as *absent here* until a peer location has been
checked. The daily sentinel that reads those archives now runs on both machines, each over its own rounds, because archives are split by machine and one sentinel would surveil only the rounds that ran where it runs.

The archive itself still never enters the repository. A committed transcript is,
by construction, an answer key — exactly the material a future adversary must
not have seen — so committing it would poison the next round's independence
while looking like good record-keeping. Round records stay committed and
append-only; the archive holds evidence only.

One consequence of freezing verdicts beside their rounds: when the grader
changes, every frozen verdict it produced is marked untrusted against the live
grader's own hash. The verdict is not re-judged in place. Discharge requires a
re-grade record from the current grader that matches the frozen file byte for
byte. That batch re-grade has not run. The step that would write the re-grade
records is not yet built on this axis, and no re-grade record exists anywhere
in its tree. Measured this refresh over every frozen independence verdict in
the tree, 48 verdicts across nine example cells: 2 read trusted, 36 read
untrusted against the live grader, and 10 predate the grader stamp and carry no
grader identity. The two trusted verdicts are this cycle's two rounds, frozen
under the grader that is live now. Nothing was re-graded to produce them, and
they will read untrusted at the next grader change like the rest. The previous
refresh's "none reads trusted" was true when written and is withdrawn. The
on-roster cells hold three of those 48, all untrusted. None of the 36 is
evidence for the tier it once supported until a re-grade discharges it.

## What a change does to the evidence already on file

Every kind of change that can land under a proved result now has a row in one
table, and each row is classed one of four ways. The evidence either
**carries** over unchanged, has to be **re-attested** by a later round, goes to
**review**, or is **void**. Some examples: a moved definition under a held
statement re-attests. A moved grader re-attests, and that is the row the
re-grade in the previous section depends on. A toolchain bump re-attests. A
breach voids. A kind with no instance on this axis is marked that way with a
stated reason. The table's lint refuses that mark on any other row, so "not
applicable" cannot be used to skip a row that does apply.

Two properties are deliberate. The table reads the axis's existing instruments
and adds no gate of its own, so it has no way to disagree with them. It also
classifies kinds of change without scheduling anything: the order in which
staged work re-lands is written into it as a dependency, not as a plan.

In the week the table landed, the axis's lint for unwired scripts flagged the
table's own lint, because nothing except its own test called it. The ruled
cure for that class is a header declaring the script an operator verb, not a
caller invented to satisfy the lint. Measured after the fix: 48 scripts in the
population, three declared, zero findings.

## A check that could not run reported OK

A shape check for conceded findings graded each artifact by whether it
elaborates green. On a checkout with no compiled package, every artifact failed
to elaborate on a missing module, and the check printed OK with nothing
elaborating. Run against a built package, the same check found ten of eleven
artifacts in one cell mis-shaped. The step that closes a round calls this
check, so it would have passed a mis-shaped round on any unbuilt tree.

The check now confirms that its imports are built before it elaborates
anything, through the same build-precondition component the axiom audit uses.
If they are not built, it exits as could-not-look: never OK, and never a
verdict. Its new witness refuses an artifact that imports a module that does
not exist, and the previous version of the check fails that witness.

**A predicate that cannot be evaluated is not a predicate that holds.** This
page has stated the rule before. This instance was the permissive direction.

## An instrument that runs inside the thing it grades

Four of the axis's instruments elaborated the code under test in their own
process: the axiom-closure probe, the statement fingerprint behind the fold
gate, the battery of generated probes, and the judge that classifies each
attack file. Lean runs a module's `initialize` blocks when it is imported with
initializers enabled, so code written by a participant ran inside the
instrument grading it. Each defect was shown red by a committed known-bad
before it was cured. An imported initializer that printed a clean transcript
and exited zero turned a proof containing `sorry` into a pass. Another turned
every generated probe green and erased a real finding. A tab character in a
declaration name shifted a record's fields, so a changed definition moved no
fingerprint. An example missing from the import graph answered "vanished"
instead of refusing.

Three of the four are now standalone programs. Each imports only Lean itself,
loads the compiled modules under test at run time with initializers never
enabled, and prints structured records that end in a count the caller
recomputes. A missing or disagreeing end record is a failure, never a pass.
Queries that used to be spliced into generated Lean source are passed as data.

The judge could not be isolated that way. Its job is to elaborate attack files
that import the proof, a real import needs initializers, and so code from both
sides runs in one process. Its verdict is now read only from a final record
built from the compiler's own messages and stamped with a nonce that the judge
reads before any imported code runs. The exit code and standard output decide
nothing. Output with no record under the right nonce is unverified, not clean.
One residue is recorded rather than claimed closed: a single command that
rewrites its own message log before returning.

Each cure was measured for equivalence against the instrument it replaced
before it landed. The axiom probe gave identical closures and verdicts on all 41
live examples. The statement fingerprint was identical on all 836 scoped
references, so no committed record moved. The battery gave 1,041 of 1,041
probes identical. The judge classified all 728 committed attack files the same
way. The judge's cure roughly doubled its cost per file. Running files in
parallel and classifying them in their original order brought one cell's full
judge from 221 seconds back to 89, against 86 before the cure.

**An instrument that executes the artifact it grades has to be shown, by a
known-bad, that the artifact cannot write its verdict.** Agreement on every
honest input is necessary, and it says nothing about that.

## A toolchain bump is graded by the judge, not the build

The kernels moved from Lean v4.34.0 to v4.35.0 on 2026-10-20. Every library and
example built green, and on both other axes every example proof with a recorded
verdict replayed to the same verdict. On this axis the build was not the test
that mattered. The attack corpus was replayed through the real judge under both
compilers, file for file, and the first pass on the new one regressed eleven
fixtures. Lean 4.35 deleted three trust-base constants, `Lean.ofReduceBool`,
`Lean.ofReduceNat` and `Lean.trustCompiler`, and eleven committed fixtures named
them. This was not an audit escape. Since 4.32, `native_decide` has minted a
per-declaration axiom instead, and the live audits already key on that shape.
But a ban list that names a constant which no longer exists bans nothing while
reading as armed, so the deleted names were dropped rather than kept. After
that, all 726 attack files classified identically under both compilers.

The bump did not land the way the README said bumps land. It went in as two
commits about fifty minutes apart: one kernel moved alone first, in a session
that held only that kernel, with the skew recorded, and the other two moved
together. The README had stated a single commit as the rule, and the rule had
never been exercised. It is corrected.

Two smaller findings came out of the same day.

- Participants launched outside the tree resolve the compiler from their own
  working directory, which is the hazard the README names, in a new place. A
  build that skipped the change of directory ran on the default compiler and
  rewrote compiled artifacts shared with sibling participants. Every launcher
  now pins the compiler from the package's own pin file and refuses to launch
  without one.
- The lane's main script located itself from the name it was invoked by. That
  is right when it is executed, and right when it is sourced from zsh, and
  wrong when it is sourced from bash. Sourced from bash during the bump's
  re-verification, it pointed at the caller's tree, a helper failed to import,
  and two standing sentinels were judged as landed attacks. That is a false red,
  which is the only reason it was noticed.

## A grader that cannot see the defect it was built for

In recent rounds an adversary has convicted prose: sentences in a proof file's
documentation that claimed more than the theorems beside them proved. The
constructive side conceded each finding at the sentence. A documentation grader
was then built. It is report-only. It checks the lead sentence of each
proposition's docstring against the statement on two shapes: a quantifier word
against the outermost quantifier, and a claim about one side of a paired
constant against the side the statement actually names. It abstains, and counts
the abstentions, where a lead is negated or names both sides. It runs a
self-test against a labelled fixture before grading anything, and a sabotaged
rule makes it refuse to grade at all.

It was measured before it was trusted, and the measurement is the useful part.
On the cell it was built for, it flagged 2 of about 650 docstrings, and both
flags were false on a hand read. Over the whole tree it read 1,200 docstrings,
34 of 41 examples came back unmeasured, and none of its 5 flags was true. Run
against the round before the conviction, it misses the convicted sentence. That
sentence was section prose, a module-level doc attached to no declaration, which
the grader counts and cannot grade. The first round after the grader landed
opened its new finding in the same kind of place.

**A grader built to answer a finding should first be run on the artifact that
produced the finding.** This one fails that test. It prints its count of
ungraded module docs on every run instead of folding them into a clean result.

## Instruments that check themselves before they report
A small pattern, stated because it is cheap and it has now caught three real
defects at first fire. Every arm of a periodic reporting check is preceded by a
self-sabotage pass over the check's own logic; if the sabotaged copy does not
fail, the run aborts before producing any verdict at all. Its first fire
convicted its own arm design twice — one arm mass-refused historical records
from before the contract it was grading existed, and a self-assertion caught a
generated baseline directory that had never been excluded from version control.
Both were found before the check ever published a number.

The same discipline applies to the witnesses: a proof-of-fire arm can be
simultaneously correct — it fails — and wrong, because it fails for a different
reason than the one it was written for. Run the sabotage and read *why* it went
red, not just that it did.

The blind adversarial cells are now launched from outside the repository. An
agent started inside the tree is handed the project's instruction files and
its memory index before it reads a single prompt. That is a leak a written
rule can declare but not prevent. A paired probe settles it: the same cell
launched inside the tree carried both kinds of material, and launched
outside, neither. A launch that has to fall back to the in-tree path records
the leak as declared, not cured.

This cycle closed the remaining inbound channel. A participant launched
outside the tree could still receive a message queued by a peer, and it could
still load tool capabilities the brief did not grant. Both are now disallowed
on every participant. The harness's queue record is read from the transcript
by its shape, so a delivered message convicts at spawn and again before the
audit hands off. The witness reds against the launcher as it stood before the
cure.

Frozen verdicts are no longer re-judged in place either. A later grader's
reading of a frozen file is appended as a separate record. That record
either confirms the original outcome or contradicts it, and the original
verdict's bytes are never rewritten.

## A verdict that is a function of where the shell was standing
The lane's independence audit convicted a participant this cycle for reading a
file outside its own surface. The file does not exist.

The command was compliant and used exactly the form the brief prescribes: change
into the working directory, then reference a neighbouring file relatively.
Resolved against that directory, the target is an ordinary, specific, permitted
file. But the resolver was handed the working directory **recorded in the
transcript** — which is the orchestrator's own shell at the moment it spawned
the participant, not the participant's. The orchestrator had stepped into a
directory the participant is banned from, in order to read source claims before
spawning it, and that location was stamped into the participant's record.
Driving the real resolver on the recorded location reproduces the convicting
string byte for byte. Both participants' recorded locations were, in fact,
backwards with respect to their own surfaces.

So a conduct verdict was a function of where an unrelated shell happened to be
standing. This is a known class — an orchestrator-authored conviction — one
layer deeper than the previous instance and invisible where that one was
legible.

Three things follow, and only the first is about this defect:

- **The verdict stands and is not argued down.** The audit is not re-run in
  search of a different answer; that is the one response the lane forbids. The
  defect is filed, not applied.
- **The instrument is shared across all three kernels**, so the other two axes
  are exposed identically. A defect in a shared component is not scoped to the
  axis that found it.
- **A shared-component fix is regression-measured against every consuming axis's
  own test suite, never against the changing axis's production run.** Measured
  this cycle: one such change reds three assertions in a sibling axis's suite,
  while the check the changing axis ran instead came back clean — because its
  production run declares none of the state the change moved. The cheaper check
  is not merely weaker; it is systematically blind to exactly this class.

One more, recorded because it is unflattering. The intervention chosen for that
round — restating the ban in full, as the opening content of the brief, with the
compliant recipe attached — did not prevent the twelfth instance of the
behaviour it was written to prevent, and was not what convicted anyway.
**Briefing has now been measured as not being the lever.** That is a result
about instructions, not about the participant.

Three more instances of the same class were cured this cycle, all in the
grader that every kernel shares:

- The text of a stream-editor substitution was read as a path argument. Its
  delimiters normalised to the filesystem root, and a recursive search later in
  the same command supplied the "recursive" signal. A compliant command that
  searched only the participant's own directory was convicted as a sweep from
  root.
- A participant re-read the harness's own overflow file for one of its own
  permitted commands. The grader convicted this as a read of another
  participant's transcript. The carve for "its own" was keyed on each call's
  recorded working directory, which the participant had legitimately changed,
  while the harness fixes the participant's project directory at launch. The
  carve also reproduced only two of the three characters the harness rewrites
  when it names that directory. Keying on the launch location, with the
  harness's full naming rule, also closed a false negative the per-call key had
  admitted: a participant that stepped into a sibling's directory could have
  claimed the sibling's overflow file as its own. A narrower pattern was
  considered and not taken, because it would have stopped convicting reads of a
  sibling's file.
- Changing into an ancestor directory and then searching a relative path into
  the participant's own output convicted the ancestor as the sweep root.

The previous section said the audit is not re-run to get a different answer,
and that still holds, so how these were resolved needs to be stated
precisely. Each defect was reproduced against the real grader. The cure was
regression-measured with known-bad and known-good cases. An operator ruled the
regrade. The frozen archive was then replayed through the cured grader, and
the result was appended as a superseding record beside the original verdict,
whose bytes are unchanged. Two rounds this cycle went from a breach verdict to
a clean or review verdict that way and were then folded. None of them is in
this page's figures, because both are on a family held off the roster.

The rule that keeps recurring: **key a channel rule on the channel's object,
and pair every known-bad with a known-good.** A rule keyed on how the access
was spelled convicts the careful caller.

Participants are now also briefed never to read an overflow file and to re-run
the command more narrowly instead. That instruction is right under either
reading of the rule it works around.

## A field with a reader and no writer is a cert that can only void
Frozen independence verdicts carry a stamp of the set of channels they were
graded against, so that a later change to that set can scope a certificate
rather than discard it. The shared reader had an arm for this scoping. No
kernel's writer had ever produced the per-channel readings it needed, so every
stamped certificate would have voided at the next channel-set change, silently
and by default. The freeze step now writes those readings. Its witness is
coupled to the real reader instead of a copy, and the stamp was executed on a
copy of a real verdict before landing.

The general form: **a field defined by its consumer and written by no producer
is inert, and an inert field fails in whatever direction its default points.**

A related roster decision was taken this cycle. The operational statement
graph, a generated emit that carries each theorem's status and documentation,
is now on the list of material a blind participant may not read. It is an
answer key. Measured before the change: none of the eight participant
transcripts in the affected rounds had read it.

## The cost of the trust
One finding from a review of the lane's own daily operation belongs here because
it is unflattering and load-bearing: **the fixed per-round overhead now exceeds
the proving work.** A round is roughly a dozen orchestrator-sequenced steps, and
nearly every one is scar tissue from a specific dated defect, each individually
justified. The composition is the problem. The honest summary is deflation on
the headline numbers and a strong net gain in how far those numbers can be
trusted — deliberate, ruled, and correct — with a cost curve for maintaining
that trust that is currently super-linear.

## A polarity trap worth publishing
One recurring mechanical trap, because it will recur anywhere a test asserts an
absence. A gap probe asserts that a diagnostic *is* produced. Close the gap and
the probe compiles clean — so the attack lane reads clean-on-annotated as
*landed*, and **the round that fixes a named gap reds itself.** There is no
"discharged" verdict to reach for. The resolution is to retire the probe into a
standing discharge record: drop the directive, keep the measurement.

## A description cannot falsify its own currency
The freshness flag behind the public card has now been repaired twice, and the
second defect is better than the first.

The first version asked whether the snapshot's revision was an *ancestor* of the
current one — which it is, and stays, forever. It could report fresh and could
never report stale.

The replacement asked a question with a reachable failing branch: has anything
changed since the snapshot was taken? It counted changed files between the
snapshot's revision and now. **The snapshot's own outputs live inside the region
it was counting, and they are committed at a revision strictly later than the
content they describe.** So the first time a regenerated snapshot was committed,
every later reading reported drift forever — a permanent, self-inflicted stale
signal, from a check that was correct in shape and wrong in domain. A description
that includes itself in the population it measures cannot report on its own
currency.

The cure is structural rather than a carve-out: recompute a digest over the
kernel sources and the compiler pin, and compare it against the digest the
snapshot stamped when it was taken. A follow-up correction was needed on the
**coordinate** — the right root is the build package, not the surrounding
project. Read from one level up, the population grows by an order of magnitude,
sweeps in every debate artefact, and picks up the wrong one of two compiler pins,
so the recomputed digest can never match the stamped one except by accident.
**Asking a well-formed question at the wrong coordinate is still the wrong
question**, and it fails in the direction that looks like a real finding.

The producer and its test now run the same code rather than two copies of it.

With that in place the flag reports current. The card first read healthy again on
2026-08-28, after reading stale since 2026-07-25, and the coverage fraction above
has been published at every refresh since.
The previous snapshot's drift count is **retired, not improved**: it was the
output of the defective instrument, and restating it smaller would have implied a
trend that the number could not carry.

One further step this cycle: the content digest is now the stamp of record,
and the revision the snapshot was taken at is a note that decides nothing. A
coverage emit is refused as dead only when it carries no digest at all. The
reader no longer consults revision ancestry, which is the question the first
defective version asked.

## Three instruments wrong toward a false clean, on one round
The first independently-audited round on a new family found three lane
instruments broken, and all three broke in the same direction — toward reporting
clean.

- A configuration file stated that the judge inspects one directory and does not
  descend into a scratch directory. The judge runs a recursive search. The
  discrepancy was proof-fired at twenty-two versus twenty-three items. **The cost
  of an instrument that under-describes itself lands on the participant who obeys
  its contract**, not on the one who ignores it.
- The judge's inference of which round a receipt belongs to mis-keys the *first*
  audited round of any example that predates the auditor — which is nearly every
  example. One code path reads the missing predecessor as "re-judge", another as
  "fold with a warning", and nothing reconciled them.
- A closure collector walked a theorem's statement and not its proof, because the
  underlying accessor returns nothing for a theorem. It reported eight names
  where the truth was eleven — and the three it missed were exactly the committed
  facts it existed to audit.

The transferable half: an instrument that fails toward clean is not found by
running it. All three were found by a round that had a reason to distrust them.

## The brief was refuted by the participant it briefed
The round after that one produced the most useful result of the cycle, and it is
a result about the orchestrator.

The session briefed the constructive side that a certain statement had a
"stronger, indexed form". That claim had been inherited from the previous round,
carried forward through a tracking item, written into the brief, and **never
checked by anyone**. The adversary derived the indexed statement
character-for-character from the unindexed one, then generalised to an arbitrary
index and instantiated it at a trivial value. **The index was inert.** The
strengthening had never existed.

The rule minted from it, and adopted across all three kernels: **a claim that one
form is stronger than another needs a proof in both directions.** Pricing only
the expensive direction is what makes the wrong answer feel measured.

A second result from the same round is less flattering and more useful. A brief
convened *specifically* on a recurring over-claiming defect produced a
generated hundred-and-eighteen-member enumeration and fourteen demotions in
place — and still shipped three fresh false ordering sentences, an
anti-vacuity binder that was inert, and a warrant that miscounted its own
environment. **A per-item audit measures diligence, not control of the
generator.** The only thing that grades control of a generator is the *next*
artefact it produces.

So the following round was deliberately reversed: its findings were **not**
pre-fixed the way the previous round's were. Cleaning up before the next round
spares the constructive side the cost of its own over-claiming, which is
precisely the thing being measured.

## Five instruments that reported green over a failure
Cured in one pass, and worth publishing as a set because the shape repeats:

- A new test suite reported PASS over a failed assertion. Its helper library
  exports one name and the suite called another, and an undefined command in a
  `|| fail` idiom does not abort — it succeeds quietly. A proof-of-fire arm was
  added; the suite had never once been shown to be capable of failing.
- A test that stages a copy of the code it exercises was staging a hand-written
  file list that had already gone stale once. It now derives the list, with an
  arm that reds if the derivation returns nothing.
- An ordering check compared the *first* textual match anywhere in a file, so a
  comment counted as a call site — and the silent inverse is worse: a comment
  mentioning the guard early would make a genuinely mis-ordered lane pass.
- Another arm pinned a retired *mechanism* rather than the property the mechanism
  was there to hold, so it kept passing after the mechanism was replaced.
- A de-duplication of four routines copied across five callers looked safe by
  reading and was not. Three of the "identical" copies differed — raw versus
  stripped command output, two string-quoting conventions that agree until the
  first value containing a quote, and a strict lookup versus a defaulting one.
  All three are preserved as separate entry points and documented as numbered
  traps. **A dedup verified by reading would have shipped all three.**

## A guard authorized and deliberately unbuilt
A kernel of machine-checked guards was authorized this cycle by minting its
contract — and it is **unstarted**, on purpose, owned by no work item. It is
recorded here because the authorization is the interesting part: the argument for
it is a failure mode, not a feature. If the guard set is built as a kernel,
incoherence in it becomes a red build; if it is built as a set of scripts,
incoherence becomes a smaller pass. **A coverage number over a stale population is
indistinguishable from one over a complete population**, which is the whole reason
to pay for the kernel.

The contract's own test suite is written to go red the moment the guard kernel
appears. The first build session has to rewrite that case into a real check
rather than let it quietly stop grading anything — which is itself the failure
mode the suite exists to name.

---

## Cadence
Re-rankings, new threads, and dropped items land as ordinary diffs; the commit
log is the change record.

## How to verify
- The 10 focus areas + reading order + skip list are the whole syllabus; every
  upstream citation resolves to a public repository.
- The textual and numerical kernels are observable in the two published kernel
  repos above; the operational kernel's theorems are described here as they
  land.
- Every count in this file is emitted by the same build that checks the proofs;
  none of it is hand-maintained. Where a count is scoped — as the adversarial
  scoreboard is — the scope is stated next to it rather than left to inference.
- Where a figure is stale, this file says stale rather than restating it. Where
  a figure is *convicted* — produced by an instrument since found defective —
  this file publishes nothing in its place and says why, rather than publishing
  the convicted value with a caveat attached.
- Where two defensible bases exist for the same count, this file names both and
  says which one it publishes.
- Every falsifiable claim on this page is re-derived against the working tree at
  each refresh, not carried forward because it was published last week. Four
  claims were corrected on that basis at the 2026-08-28 refresh, three at the
  next, at the one after, the adversarial block itself, which had been
  published one fold behind, along with a cross-reference from the README to
  a section that did not exist. At the 2026-10-11 refresh, three corrections: the header's statement that no
  round had run since 2026-08-28 (rounds had run and folded, all off the roster),
  the held-off family count (six, now ten), and the README's account of how a
  toolchain bump lands. At this one, two: the statement that seven retirements
  were in no metric until the next clean round (they entered their cell's
  standing at its next fold, on 2026-08-16, and that cell is off the roster), and
  a held-off qualifier that described the previous cycle as this one. A third
  carried claim, that the verdict re-grade has not run, was re-measured and
  stands. It now carries its population. At the 2026-10-23 refresh, five: the
  README's account of how a bump lands (it stated a rule that had never been
  exercised, and the next bump did not land that way); the README's count of
  releases between the metaprogramming book and the kernels (right at the pin
  it was written against, wrong since the bump after, and now stated as two
  versions instead of a derived count); the README's statement that the lane's
  live target had moved to a newer family (it moved back); this page's
  statement that no frozen verdict reads trusted (two now do); and this page's
  description of a landing-day population as today's. The first four were true,
  or untested, when written. The last was a basis error.

## Contact
[github.com/quantapix](https://github.com/quantapix) — open an issue on any repo
in the org. Answered in public; there is no contact email.
