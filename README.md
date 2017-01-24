# cSpell-WordLists
Word Lists that can be used with the cSpell Spelling Checker

## Setup
To be able to convert raw dictionary files, you have to set things up.

```
npm install
```

## Raw Dictionaries

These are the source word lists.  Put new files here: `./raw-dictionaries`

## Processing Raw Dictionaries

To build all the dictionaries:

```sh
npm run build-all
```

To build a single dictionary.

### Example: build php.txt
```sh
npm run build ./raw-dictionaries/php.txt
```

### List Run commands:
```
npm run
```

## Building a Hunspell Dictionary

1. Extract the words: <br/>
   ```npm run hunspell-reader -- words ./hunspell/nl.dic -o ./raw-dictionaries/wordsNl.txt```
2. Normalize the word list: <br />
   ```npm run build ./raw-dictionaries/wordsNl.txt```

It can take a long time to process all the words.

## Using the Hunspell-reader

The Hunspell-reader will read the Hunspell `.dic` and `.aff` files and output a list of words.

If you install the hunspell-reader globally, then things are a bit simpler:

```
npm install -g hunspell-reader
```

### Extract the words:
```
hunspell-reader words ./hunspell/nl.dic -o ./raw-dictionaries/wordsNl.txt
```

### Getting Help
See [github: hunspell-reader](https://github.com/Jason3S/hunspell-reader)

```
hunspell-reader words --Help
```


