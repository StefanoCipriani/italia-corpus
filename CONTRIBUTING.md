# Contributing to Italia Corpus

[🇬🇧 English](#english) · [🇮🇹 Italiano](#italiano)

---

## English

Thank you for your interest in contributing. This project has two separate repositories with different scopes:


| Repository                                                              | What it contains                   | Where to contribute                            |
| ----------------------------------------------------------------------- | ---------------------------------- | ---------------------------------------------- |
| [italia-corpus](https://github.com/ahmeabd/italia-corpus)               | The corpus itself (Markdown files) | Issues about missing or malformed acts         |
| [italia-corpus-script](https://github.com/ahmeabd/italia-corpus-script) | The open-source pipeline script    | Code improvements, parsing fixes, new features |


### Reporting issues

- **Malformed or missing act** → open an issue on [italia-corpus](https://github.com/ahmeabd/italia-corpus) and include the URN or `codice_redazionale` of the affected act.
- **Parsing bug or pipeline error** → open an issue on [italia-corpus-script](https://github.com/ahmeabd/italia-corpus-script) with a short reproduction case.
- **General question or suggestion** → reach out at [ahmeabd36@gmail.com](mailto:ahmeabd36@gmail.com).

### Pull requests

Pull requests are welcome on [italia-corpus-script](https://github.com/ahmeabd/italia-corpus-script) for:

- Parsing fixes and accuracy improvements
- Validation scripts
- Tooling integrations (loaders, indexers, converters)
- Documentation

**Before opening a PR that changes the on-disk format** (frontmatter fields, file naming, directory layout), please open an issue first so the change can be discussed. Format changes affect every downstream integration.

### Frontmatter & metadata

The YAML frontmatter in each file is the primary integration surface of this corpus. If you believe a field is missing, misnamed, or incorrectly populated, open an issue with:

1. An example URN or file path
2. The current value
3. The expected value and why

Do not submit PRs that strip or reorder frontmatter fields without prior discussion.

### Corpus content

The Markdown content of each act is derived automatically from Normattiva. Edits to individual `.md` files will be overwritten on the next pipeline run. If you spot a content error, report it upstream through the script repository so the fix is applied at the source.

---

## Italiano

Grazie per il tuo interesse a contribuire. Il progetto è diviso in due repository con scopi distinti:


| Repository                                                              | Cosa contiene                        | Dove contribuire                                            |
| ----------------------------------------------------------------------- | ------------------------------------ | ----------------------------------------------------------- |
| [italia-corpus](https://github.com/ahmeabd/italia-corpus)               | Il corpus (file Markdown)            | Issue su atti mancanti o malformati                         |
| [italia-corpus-script](https://github.com/ahmeabd/italia-corpus-script) | Lo script open source della pipeline | Miglioramenti al codice, fix di parsing, nuove funzionalità |


### Segnalare problemi

- **Atto malformato o mancante** → apri una issue su [italia-corpus](https://github.com/ahmeabd/italia-corpus) indicando URN o `codice_redazionale` dell'atto interessato.
- **Bug nel parsing o errore nella pipeline** → apri una issue su [italia-corpus-script](https://github.com/ahmeabd/italia-corpus-script) con un caso di riproduzione.
- **Domanda generale o suggerimento** → scrivi a [ahmeabd36@gmail.com](mailto:ahmeabd36@gmail.com) o crea una disucssion.

### Pull request

Le PR sono benvenute su [italia-corpus-script](https://github.com/ahmeabd/italia-corpus-script) per:

- Fix di parsing e miglioramenti all'accuratezza
- Script di validazione
- Integrazioni (loader, indicizzatori, convertitori)
- Documentazione

**Prima di aprire una PR che modifica il formato su disco** (campi del frontmatter, naming dei file, struttura delle directory), apri una issue per discuterne. Le modifiche al formato impattano tutte le integrazioni esistenti.

### Frontmatter e metadati

Il frontmatter YAML di ogni file è la principale superficie di integrazione del corpus. Se ritieni che un campo sia mancante, mal nominato o valorizzato in modo errato, apri una issue con:

1. URN o percorso del file di esempio
2. Il valore attuale
3. Il valore atteso e la motivazione

Non inviare PR che rimuovono o riordinano i campi del frontmatter senza discussione preventiva.

### Contenuto del corpus

Il contenuto Markdown di ogni atto è derivato automaticamente da Normattiva. Le modifiche dirette ai file `.md` vengono sovrascritte alla successiva esecuzione della pipeline. Se noti un errore nel contenuto, segnalalo attraverso il repository dello script in modo che la correzione venga applicata alla fonte.