# PGN-parser

A Portable Game Notation (PGN) ANTLR 4 grammar and parser.

The grammar can be found in 
[`src/main/antlr4/nl/bigo/pp`](https://github.com/DennisPiskovatskov/PGN-parser/tree/master/src/main/antlr4/nl/bigo/pp).

Seeing the generated parser in action can be done by building
a *fat* JAR of the project and then running it to parse a PGN
file. A couple PGN files reside in 
[`src/resources`](https://github.com/DennisPiskovatskov/PGN-parser/tree/master/src/resources).

# Get started

### 0. Clone this repository

```bash
git clone https://github.com/DennisPiskovatskov/PGN-parser
cd PGN-parser
```

### 1. Generate the lexer and parser classes

```bash
mvn clean antlr4:antlr4
```

### 2. Build the *fat* JAR

```bash
mvn install package
```

### 3. Parse a PGN file

```bash
java -jar target/pp-0.1.1-SNAPSHOT.jar src/resources/Karpov.pgn
```
