# Diddy Neko's Numco Decipher

🌐 **Live Web App:** **[https://ifung-0.github.io/numco-decipher/](https://ifung-0.github.io/numco-decipher/)**

**Diddy Neko's Numco Decipher** is an interactive encoder, decoder, and auto-cracking web tool for **Numco (Numco 100%)**—a 4-column mobile keyboard symbol substitution cipher and QWERTY-shift system.

---

## 📖 How the Numco System Works

At its core, **Numco** maps the 26 letters of the English alphabet in **QWERTY keyboard order** (`q` through `m`) to four distinct columns of numbers and symbols found across mobile keyboard layers:

1. **1st Column:** Simple Numco
2. **2nd Column:** Numco
3. **3rd Column:** Advanced Numco
4. **4th Column:** Gay Numco

### The QWERTY Sequence Rule

Whenever a Numco method shifts letters forward (`+`) or backward (`-`), it **always** shifts along the **QWERTY keyboard sequence**, *never* standard `A–Z` alphabetical order:

```text
qwertyuiopasdfghjklzxcvbnm
```

| Position | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 | 13 |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Letter** | `q` | `w` | `e` | `r` | `t` | `y` | `u` | `i` | `o` | `p` | `a` | `s` | `d` |

| Position | 14 | 15 | 16 | 17 | 18 | 19 | 20 | 21 | 22 | 23 | 24 | 25 | 26 |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Letter** | `f` | `g` | `h` | `j` | `k` | `l` | `z` | `x` | `c` | `v` | `b` | `n` | `m` |

* **Wrapping Around:** The sequence wraps seamlessly at both ends. Shifting `m` forward by `+1` wraps around to `q`, and shifting `q` backward by `-1` wraps around to `m`.
* **Spaces:** Spaces between words are always kept unchanged.

---

## 🔑 Official Numco Alphabet Key (`q` -> `m`)

### Raw Copyable Key Block

```text
q = 1 = ¹ = ~ = ~
w = 2 = ² = ` = `
e = 3 = ³ = | = |
r = 4 = ⁴ = • = ♪
t = 5 = ⁵ = √ = √
y = 6 = ⁶ = π = Ω
u = 7 = ⁷ = ÷ = ÷
i = 8 = ⁸ = × = ×
o = 9 = ⁹ = § = ¶
p = 0 = ⁰ = ∆ = ∆
a = @ = @ = £ = £
s = # = № = ¢ = ¢
d = $ = ¢ = € = €
f = _ = _ = ¥ = ¥
g = & = & = ^ = ↑
h = - = — = ° = ′
j = + = ± = = = ∞
k = ) = > = } = )
l = ( = / = \ = \
z = / = † = % = ‰
x = * = ” = © = ©
c = " = ’ = ® = ®
v = ' = : = ™ = ™
b = : = ; = ✓ = ✓
n = ; = ¡ = [ = [
m = ? = ¿ = ] = ]
```

### 4-Column Reference Table

| # | Letter | Col 1: Simple Numco | Col 2: Numco | Col 3: Advanced Numco | Col 4: Gay Numco |
| :---: | :---: | :---: | :---: | :---: | :---: |
| 1 | **q** | `1` | `¹` | `~` | `~` |
| 2 | **w** | `2` | `²` | `` ` `` | `` ` `` |
| 3 | **e** | `3` | `³` | `\|` | `\|` |
| 4 | **r** | `4` | `⁴` | `•` | `♪` |
| 5 | **t** | `5` | `⁵` | `√` | `√` |
| 6 | **y** | `6` | `⁶` | `π` | `Ω` |
| 7 | **u** | `7` | `⁷` | `÷` | `÷` |
| 8 | **i** | `8` | `⁸` | `×` | `×` |
| 9 | **o** | `9` | `⁹` | `§` | `¶` |
| 10 | **p** | `0` | `⁰` | `∆` | `∆` |
| 11 | **a** | `@` | `@` | `£` | `£` |
| 12 | **s** | `#` | `№` | `¢` | `¢` |
| 13 | **d** | `$` | `¢` | `€` | `€` |
| 14 | **f** | `_` | `_` | `¥` | `¥` |
| 15 | **g** | `&` | `&` | `^` | `↑` |
| 16 | **h** | `-` | `—` | `°` | `′` |
| 17 | **j** | `+` | `±` | `=` | `∞` |
| 18 | **k** | `)` | `>` | `}` | `)` |
| 19 | **l** | `(` | `/` | `\` | `\` |
| 20 | **z** | `/` | `†` | `%` | `‰` |
| 21 | **x** | `*` | `”` | `©` | `©` |
| 22 | **c** | `"` | `’` | `®` | `®` |
| 23 | **v** | `'` | `:` | `™` | `™` |
| 24 | **b** | `:` | `;` | `✓` | `✓` |
| 25 | **n** | `;` | `¡` | `[` | `[` |
| 26 | **m** | `?` | `¿` | `]` | `]` |

---

## 🧩 The 6 Official Methods of Writing in Numco

### Method 1: Normal Numco
Choose **one column** and use only symbols from that column for the entire message. You cannot switch between columns halfway through.
* If you start with Column 1, stay with Column 1. If you start with Column 2, stay with Column 2, and the same rule applies to Columns 3 and 4.
* **Examples (`"hi"`):**
  * Column 1: `-8`
  * Column 2: `—⁸`
  * Column 3: `°×`
  * Column 4: `′×`
* **Example (`"hello"` in Column 1):**
  * `h` -> `-`, `e` -> `3`, `l` -> `(`, `l` -> `(`, `o` -> `9` => **`-3((9`**

---

### Method 2: Alternating Numco
Alternate between different columns for consecutive letters in a consistent repeating pattern. Each symbol must come from a different column than the symbol immediately before it.
* For example, use Column 1 for the 1st letter, Column 3 for the 2nd, Column 1 for the 3rd, Column 3 for the 4th, and repeat that pattern throughout the message.
* **Example (`"hi"` alternating Column 1 and Column 3):**
  * `h` uses Column 1 (`-`)
  * `i` uses Column 3 (`×`)
  * Result: **`-×`**

---

### Method 3: Shifted Numco (`+1` or `-1`)
Choose **one of the 4 columns** and stick to it for the entire message, just like Normal Numco. Before encoding each letter, shift it one position **forward (`+1`)** or **backward (`-1`)** in the QWERTY sequence (`qwertyuiopasdfghjklzxcvbnm`), and then encode the shifted letter using your chosen column.
* **`+1` Numco:** Shift every letter 1 position forward in the QWERTY sequence (e.g., `h` becomes `j`, `e` becomes `r`, `l` becomes `z`, `o` becomes `p`).
* **`-1` Numco:** Shift every letter 1 position backward in the QWERTY sequence (e.g., `h` becomes `g`, `e` becomes `w`, `l` becomes `k`, `o` becomes `i`).
* **Examples for `"hello"` (using Column 1):**
  * Normal Numco: **`-3((9`** *(or `-3//9` in Column 2 for `l`)*
  * `-1` Shifted Numco: `hello` -> `gwkki` => **`&2))8`**
  * `+1` Shifted Numco: `hello` -> `jrzzp` => **`+4//0`**

---

### Method 4: Plus-Shifted Numco (`+`)
Stick to **one column** for the entire message. Shift letters **forward** in the QWERTY sequence (`qwertyuiopasdfghjklzxcvbnm`) before encoding, increasing the forward shift distance by `+1` for each subsequent letter (`+1, +2, +3, +4...`).
* The `+` symbol inside an encoded message is an actual encoded character (`j` in Column 1), not a label.
* **Screenshot Example (`"hello"`):** **`+4':_`**

---

### Method 5: Minus-Shifted Numco (`-`)
Works the same way as Method 4, except you shift letters **backward** in the QWERTY sequence (`qwertyuiopasdfghjklzxcvbnm`) before encoding, increasing the backward shift distance by `1` for each subsequent letter (`-1, -2, -3, -4...`).
* Just like Method 3 and Method 4, you must stick to **one column** for the entire message.
* The `-` symbol inside an encoded message is an actual encoded character (`h` in Column 1), not a label.
* **Screenshot Example (`"hello"`):** **`&1+-4`**

---

### Method 6: Chaotic Numco (Ultimate Mode)
The hardest Numco method. It combines **column switching**, **QWERTY shifting**, and a **changing shift distance** in three synchronized 8-step repeating cycles:

1. **Column Sequence (repeats every 8 letters):**
   `Col 1 -> Col 3 -> Col 2 -> Col 4 -> Col 4 -> Col 2 -> Col 3 -> Col 1`
2. **Shift Direction Pattern:**
   `+ -> - -> + -> + -> - -> + -> - -> +`
3. **Shift Distance Pattern (repeats every 8 letters):**
   `+1, -2, +3, +1, -2, +3, -1, +2`

#### Step-by-Step Walkthrough Example Using `"zenkawa"`:
1. **Assign the column and shift to each letter:**
   * Letter 1 (`z`): use **Column 1** and shift **`+1`**
   * Letter 2 (`e`): use **Column 3** and shift **`-2`**
   * Letter 3 (`n`): use **Column 2** and shift **`+3`**
   * Letter 4 (`k`): use **Column 4** and shift **`+1`**
   * Letter 5 (`a`): use **Column 4** and shift **`-2`**
   * Letter 6 (`w`): use **Column 2** and shift **`+3`**
   * Letter 7 (`a`): use **Column 3** and shift **`-1`**
2. **Shift each letter along `qwertyuiopasdfghjklzxcvbnm`:**
   * `z` `+1` -> `x`
   * `e` `-2` -> `q`
   * `n` `+3` -> `f`
   * `k` `+1` -> `l`
   * `a` `-2` -> `m`
   * `w` `+3` -> `r`
   * `a` `-1` -> `p`
   * Shifted letter sequence: **`xqflmrp`**
3. **Encode each shifted letter using its assigned column:**
   * `x` -> Column 1: `*`
   * `q` -> Column 3: `~`
   * `f` -> Column 2: `_`
   * `l` -> Column 4: `\`
   * `m` -> Column 4: `]`
   * `r` -> Column 2: `⁴`
   * `p` -> Column 3: `∆`
4. **Final Chaotic Numco Output:** **`*~_\]⁴∆`**

---

## 🛠️ Website Features

* **Two-Way Instant Translation:** Switch between **Decipher (Numco -> ABC)** and **Encode (ABC -> Numco)** or swap inputs and outputs in one click.
* **Auto-Crack Scanner:** Displays live decoded previews across all 6 Numco methods simultaneously so you can immediately spot which method an unknown message uses.
* **Step-by-Step Symbol, Column & Shift Breakdown:** Shows the exact column, QWERTY shift distance, intermediate shifted letter, and final character for every token.
* **Copyable Discord Proof Log:** Generates a formatted step-by-step walkthrough log ready to paste directly into Discord.
* **Interactive QWERTY Sequence Strip:** Click any letter on the `qwertyuiopasdfghjklzxcvbnm` bar to inspect its `±1`, `±2`, and `±3` shifts.
* **Interactive 4-Column Chart:** Click any symbol in the reference table to insert it directly into your message.

---

## 📁 Repository Files

* `index.html` — Complete single-file application (HTML, Tailwind CSS, and JavaScript cipher engine).
* `icon.png` — Site icon (automatically cropped and centered onto the chibi Neko character for both the header avatar and browser favicon).
* `README.md` — Documentation and full Numco system reference guide.
