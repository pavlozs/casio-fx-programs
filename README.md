# Casio fx Programs

Programs for Casio fx series programmable calculators, written in Casio BASIC.

Each program comes as a plain-text listing you can type into the calculator,
together with a short guide that explains what it does, what it asks for and
what it shows.

## Programs

| Program | Calculator | What it does |
|---------|------------|--------------|
| [Triangle Solver](fx-9750GA-PLUS/triangle-solver/) | fx-9750GA PLUS | Solves a triangle from any sufficient set of sides and angles, draws it to scale and lists all sides, angles and the area. |

## How the repository is organized

```
fx-9750GA-PLUS/              one folder per calculator model
└── triangle-solver/         one folder per program
    ├── README.md            what the program does and how to use it
    └── TRIANGLE.txt         the program listing
```

Programs are filed under the calculator they were written for and tested on.
Many will also run on related models, sometimes with small changes.

## Getting a program into your calculator

1. Open the program's folder and read its `README.md`.
2. On the calculator, go to the **PRGM** mode from the main menu and create a
   new program. Use the name given in the program's guide.
3. Type in the listing from the `.txt` file line by line, pressing `EXE` at
   the end of each line.
4. Leave the editor and run the program from the program list.

### Reading a listing

A listing shows the program exactly as it appears in the calculator's editor.
Two things are worth knowing before you start typing:

**Commands are single keys or menu items, not typed letters.** Words such as
`If`, `Then`, `For`, `Next`, `Goto`, `List`, `Text`, `F-Line` or `ViewWindow`
are each one command that you pick from the calculator's menus. Only the text
between quotation marks is typed letter by letter.

**Some symbols are written with look-alike characters**, because the
calculator's own symbols do not exist on a computer keyboard:

| In the listing | On the calculator |
|----------------|-------------------|
| `→`            | Store a value in a variable (the `→` key) |
| `⇒`            | "If true, do the next command" (`PRGM` › `JUMP`) |
| `=` `≠` `>` `<` `≥` `≤` | Comparisons (`PRGM` › `REL`) |
| `?`            | Ask the user for a value (`PRGM`) |
| `:`            | Separates two commands on one line (`PRGM`) |
| `×` `÷`        | The multiply and divide keys |
| `√` `²`        | The square root and square keys |
| `sin⁻¹` `cos⁻¹` `tan⁻¹` | Inverse trigonometric functions (`SHIFT` + `sin` / `cos` / `tan`) |

Spaces in a listing are only there to make it readable. You do not need to
type them, except inside quotation marks.

## Language

Everything here is in English, including the messages the programs show on
the calculator's display.
