# cSpell-WordLists
Word Lists that can be used with the cSpell Spelling Checker

## Setup
To be able to convert raw dictionary files, you have to set things up.

```
npm run install
```

## Raw Dictionaries

These are the source word lists.  Put new files here: `./raw-dictionaries`

## Processing Raw Dictionaries

To build all the raw dic

```sh
npm run build-all
```

To build a single dictionary.

### Example: build php.txt
```sh
npm run build ./raw-dictionaries/php.txt
```


