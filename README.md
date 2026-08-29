# seed

Offline BIP-39 phrases from things you can hold: one six-sided die, one 52-card deck, or two 52-card decks.

Open **[create-seed.html](create-seed.html)** first. Pick the source you have. Next page is Basic (words only) or Full (words, first three `bc1` addresses, account `zpub`, SeedQR).

Each HTML file is the whole program. No network, no extra scripts, no browser storage, no `crypto.subtle`. Copy one file to a machine that stays offline. Open it as `file://`. Wait for the green self-test. Write the words by hand. Check them on a second device before any coins move.

**Do not generate a seed from this GitHub page, from a raw URL, or from GitHub Pages.** Download the Release zip, check the hashes, then work offline.

Current drop: **v1.0.0**.

## Layout

```
create-seed.html
dice-to-seed/          one d6
avb-52/                one deck
seedphrase-poker/      two decks
```

Keep the folders together or the back links and Basic/Full links break. Eighteen-word phrases are not offered.

## Download

Prefer the zip on [Releases](https://github.com/avbpodcast/seed/releases), not a file copied out of `main` by hand.

After you unpack:

```
sha256sum -c SHA256SUMS.txt
```

On macOS: `shasum -a 256 -c SHA256SUMS.txt`. Check again on the offline machine.

## Before funds

Restore the phrase on a hardware wallet or a second BIP-39 tool and confirm the same first receive address. Two implementations agreeing is the check. A tool agreeing with itself is not.

None of these files can judge a die or a shuffle. That part is yours.

## License

GNU GPL v3. See [LICENSE](LICENSE) on this repository.
