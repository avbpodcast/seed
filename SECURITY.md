# Security

These files turn physical entropy into a BIP-39 phrase. Treat a report that changes the words, leaks the words, or talks to the network as urgent.

## How to use a file safely

1. Download a GitHub Release zip. Do not open a raw `.html` URL.
2. Check `SHA256SUMS.txt` against the files on disk.
3. Copy one HTML file to a machine that stays offline.
4. Open it as `file://`. The self-test banner must be green.
5. Generate. Write the words on paper. Close the browser.
6. Restore on a hardware wallet or a second BIP-39 tool and compare addresses.

The green banner means this copy matched the built-in vectors. It does not prove the file was never edited. The hash is that check.

## What this repo will not do

- Host the generators on GitHub Pages
- Fetch scripts, fonts, or wordlists from the network
- Write the phrase to `localStorage`, cookies, or disk
- Call `crypto.subtle` (Full files do the extra math in plain JavaScript inside the file)

## Reporting a problem

Use GitHub’s private vulnerability reporting on this repository. Include:

- which file and which SHA-256 you hashed
- whether the self-test was green
- the exact input (rolls or cards) and what you expected
- a second-tool result if you have one
- email: security@avbforge.com

Do not paste a live seed that still holds funds.
