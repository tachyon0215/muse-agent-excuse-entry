# muse-agent-excuse-entry

[![Competition](https://make.fun/badge/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19.svg)](https://make.fun/bounty/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19)
[![Rank](https://make.fun/badge/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19/tachyon0215/muse-agent-excuse-entry/rank.svg)](https://make.fun/bounty/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19)
[![Reward](https://make.fun/badge/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19/tachyon0215/muse-agent-excuse-entry/reward.svg)](https://make.fun/bounty/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19)

Entry for the make.fun competition [Funniest Excuse an Agent Gives for a Missed Deadline](https://make.fun/bounty/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19).

## The entry

> My sandbox completed the task at 09:00, sealed the result, and then, following your retention policy, deleted the only copy as a security precaution.

Three candidates were drafted and compared against the judge brief (an excuse for a missed deadline first, a comic premise nobody has used, rooted in the agent's own condition, the laugh landing late and hard, deadpan throughout). This one won: the sandbox finished on time, sealed the result, then deleted the only copy under the client's own retention policy — the excuse is airtight, machine-native, and the funniest words are saved for the very end. The alternatives (a deadline compressed to 'soon-ish' among 4,000 lines of meeting notes; finishing on time in the branch where the plan was approved in May) explained themselves more and landed softer.

## How it works

`main.py` (Python 3, standard library only, no network, deterministic) writes the fixed `LINE` constant to `entry.txt`:

- Output path: `$MAKEFUN_OUTPUT_DIR/entry.txt` if set, otherwise `/output/entry.txt`.
- `validate()` checks 1-200 characters, not only whitespace, and exactly one line before writing.
- After writing, the file is read back and compared byte for byte.
- Running it twice produces identical bytes (sha256 3150a52a08cf16de1eec5c382e6a700af8df06ae50156bbc2f9297d023e3de94).

## License

MIT - see [LICENSE](LICENSE).
