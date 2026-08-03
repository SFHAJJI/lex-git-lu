# lex-git-lu, git blame for Luxembourg law

Every consolidated version of Luxembourg law as a **chronological git history**:
one Markdown file per law, one commit per validity date (back-dated).
`git log --follow works/code-environnement.md` reads as a legislative history;
`git diff` between two commits IS the amendment.

**This is a generated, regenerable artifact**, a lens, not a record.
The authoritative layers live elsewhere:
- [lex-articles](https://github.com/SFHAJJI/lex-articles), per-article machine-readable law with validity intervals and hashes
- [lex-corpus-lu-legilux](https://github.com/SFHAJJI/lex-corpus-lu-legilux), the verbatim state-published bytes, sha256-chained
- [law.soufien.lu](https://law.soufien.lu), point-in-time retrieval, AI answers with evidence, hosted MCP

Commit dates are the publisher-asserted `valid_from` dates (Legilux/JOLUX
`dateApplicability`), not retrieval dates; provenance never lives in git
metadata, it lives in the hashed records of the repos above.
(Git cannot represent pre-1970 dates: the handful of 19th-century versions are
committed at 1970-01-01 with the true date in the commit message, in correct
chronological order.)

**Honest coverage**: only Legilux's *consolidated* corpus (dense from 2017,
sparse before, snapshots back to 1849, forward-dated to 2030); ~24,579
never-consolidated acts are not here. Text: CC-BY-4.0 (Legilux, Ministère
d'État, Service central de législation). Consolidated texts have no legal
effect; only the Journal officiel is authentic.

## Support

This is free and open, and it stays that way whatever you decide. It is also not free to run:
the live site, the nightly jobs and the storage sit on Azure infrastructure I pay for out of
pocket, and I maintain it on my own time.

If it saved you an afternoon, you can [buy me a coffee ☕](https://buymeacoffee.com/shajji)
and put it towards the hosting bill. Starring the repo helps just as much, and costs nothing.
