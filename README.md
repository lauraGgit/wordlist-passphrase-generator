# wordlist-passphrase-generator

This is a simple passphrase generator.

It uses the long wordlist created by [Joseph Bonneau](https://www.eff.org/deeplinks/2016/07/new-wordlists-random-passphrases) for [Electronic Frontier Foundation](https://www.eff.org) to assemble a passphrase according to the [dice-based guidelines provided by EFF](https://www.eff.org/dice).

**Important:** Using this generator is [not as secure](http://world.std.com/~reinhold/dicewarefaq.html#electronic) as using physical dice.

**I have absolutely no affiliation with EFF. But I do think they do important work well, and I hope you will consider [donating to them](https://supporters.eff.org/donate/button).**

[See also.](https://xkcd.com/936/)

## Installation
```bash
pip install wordlist_passphrase_generator
```

## Usage

From the command line:
```bash
wordlist-passphrase-generator
```

From package:
```bash
import wordlist_passphrase_generator
```

- With prompt:
  ```bash
  wordlist-passphrase-generator.passphrase()
  ```

- Without prompt, where n is the number of words:
  ```bash
  wordlist-passphrase-generator.get_passphrase(n)
  ```

## Next Steps
- Use [secrets](https://docs.python.org/3/library/secrets.html#module-secrets).
- Allow user to select from a variety of wordlists.
  - [Diceware](http://world.std.com/~reinhold/diceware.wordlist.asc)
  - languages other than English
- Allow user to enter their own wordlist URI (ahem, @lauraGgit) & detect file format.
