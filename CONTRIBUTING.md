# Come contribuire al repository

## Prima installazione

Dopo aver clonato il progetto:

```bash
npm i
```

per installare le librerie

## Formattazione

Tutti i file markdown devono essere formattati con [Prettier](https://prettier.io/) per una miglior leggibilità e per evitare inutili merge conflict se più persone lavorano allo stesso file.

Per formattare da linea di comando tutti i file è necessario avere [Node](https://nodejs.org/it) installato sul proprio computer e lanciare il seguente comando nella cartella del repository:

```bash
npm run format:write
```

Fortunatamente i principali IDE supportano Prettier tramite delle estensioni, di seguito alcuni esempi:

### Visual Studio Code

Per formattare i file markdown con Visual Studio Code è necessario installare l'estensione [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode).

Un buon consiglio è tenere attivo il flag `Format On Save` direttamente nelle impostazioni di vscode per evitare di dover formattare ogni volta a mano.

### JetBrains IDE (WebStorm, IntelliJ, ecc.)

Per formattare i file markdown con IDE JetBrains è necessario installare l'estensione [Prettier](https://plugins.jetbrains.com/plugin/10456-prettier), tranne per WebStorm che include già Prettier di default.

Alcuni suggerimenti di configurazione si possono trovare [qui](https://prettier.io/docs/en/webstorm).

### Vim

Per formattare i file markdown con Vim è necessario installare il plugin [vim-prettier](https://github.com/prettier/vim-prettier).

Alcuni suggerimenti di configurazione si possono trovare [qui](https://prettier.io/docs/en/vim).

### Altri IDE

Nella documentazione di Prettier sono presenti le istruzioni per configurare il tool nel proprio IDE preferito: [Editor Integration](https://prettier.io/docs/en/editors).

## Conventional commits

Per mantenere uno storico e poter costruire dei changelog è richiesto a tutti i contributori del progetto di utilizzare i [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).  
In pratica è necessario utilizzare dei prefissi per i commit che indicano il tipo di commit e il contesto, ad esempio:

```bash
git commit -m "feat: aggiunta nuova pagina"
```

## Lingua e contenuti

Il libro è, in questo momento, orientato ad un pubblico italiano.  
Volendo essere accessibile alla platea più ampia possibile, è necessario utilizzare un linguaggio semplice e chiaro, espresso in lingua italiana, per i contenuti, le cartelle, i commit, le Pull Requests, i commenti, ecc.  
Seppur abituati a scrivere in inglese commit e Pull Requests, richiediamo a chi contribuisce di utilizzare la lingua italiana anche in questi casi, _al netto del `<type>` dei commit_ per seguire i [Conventional Commits](#conventional-commits), che resteranno in inglese.

Per quanto riguarda i capitoli del libro, è stata già predisposta una futura integrazione di ulteriori lingue (traduzioni) utilizzando un approccio `language driven` per la struttura delle cartelle. Si avrà quindi, ad esempio: `docs/it/nome-del-capitolo.md` per la lingua italiana, `docs/en/name-of-the-chapter.md` per l'inglese, e così via.

> [!NOTE]  
> Il nome del file (`nome-del-capitolo.md`) rappresenta, a tutti gli effetti, lo `slug` dell' url. Cercando sempre di mantenere una nomenclatura efficace e concisa (esempio: ✅ `sviluppo-mobile` e non ❌ `capitolo-sulle-metodologie-di-sviluppo-per-applicazioni-mobile`), è necessario utilizzare la convenzione di nomenclatura `Kebab case` (quindi parole in minuscolo separate da un `-`).

## Linee Guida

Prima di stendere contenuti o proporre delle Pull Request si suggerisce di dare una lettura alle [Linee Guida](https://github.com/Il-Libro-Open-Source/book/blob/main/GUIDELINES.md) (E relativo [Cheatsheet](https://github.com/Il-Libro-Open-Source/book/blob/main/GUIDELINES-CHEATSHEET.md)) da rispettare quando si interagisce con il repository.
