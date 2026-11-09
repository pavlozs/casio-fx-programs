# Triangle Solver

Solves a general triangle from any sufficient combination of sides and angles,
then draws it to scale and lists all sides, all angles and the area.

- **Calculator:** Casio fx-9750GA PLUS
- **Program name:** `TRIANGLE`
- **Source:** [TRIANGLE.txt](TRIANGLE.txt)

## Notation

```
            GA
            /\
           /  \
        B /    \ A
         /      \
        /________\
      AL    C     BE
```

| Label | Meaning                         |
|-------|---------------------------------|
| `A`, `B`, `C` | Sides                   |
| `AL`  | Angle alpha, opposite side `A`  |
| `BE`  | Angle beta, opposite side `B`   |
| `GA`  | Angle gamma, opposite side `C`  |
| `S`   | Area                            |

The calculator has no Greek letters, so the angles are written as the
two-letter abbreviations `AL`, `BE` and `GA`.

## Usage

1. Run the program. It asks for six values in turn:
   `SIDE A`, `SIDE B`, `SIDE C`, `ANGLE ALPHA`, `ANGLE BETA`, `ANGLE GAMMA`.
2. Enter the values you know and **enter `0` for every unknown**.
   Angles are in degrees (the program switches the calculator to `Deg`).
3. The program draws the triangle and prints the results next to it,
   rounded to two decimal places.

### Supported input combinations

| Known values                         | Case |
|--------------------------------------|------|
| Three sides                          | SSS  |
| Two sides and the angle between them | SAS  |
| Two sides and an angle opposite one  | SSA  |
| One side and any two angles          | ASA / AAS |

In the SSA case two different triangles can match the input. When that
happens the program asks `OBTUSE ANGLE? 1=YES` — enter `1` for the solution
with the obtuse angle, anything else for the acute one.

### Messages

| Message            | Meaning                                              |
|--------------------|------------------------------------------------------|
| `NOT ENOUGH DATA`  | The entered values do not determine a triangle (for example three angles and no side). |
| `NO SUCH TRIANGLE` | No triangle exists with the entered values.          |

## Example

Input: `SIDE A = 3`, `SIDE B = 4`, `SIDE C = 5`, all angles `0`.

Output:

```
A=3
B=4
C=5
AL=36.87
BE=53.13
GA=90
S=6
```

## Side effects

The program overwrites:

- variables `A`–`G`, `I`–`N` and `P`–`Z` (everything except `H` and `O`),
- `List 1`,
- the View Window, and it turns the graph axes and labels off,
- the angle unit, which is set to `Deg`.
