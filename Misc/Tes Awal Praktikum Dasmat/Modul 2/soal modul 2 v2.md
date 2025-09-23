1] Untuk setiap pernyataan di bawah, tentukan kebenarannya.
- Simbol `∀` berarti "untuk setiap".
  **Jawab: Benar**
- Simbol `∃` berarti "untuk setiap".
  **Jawab: Salah**
- Pernyataan `x y : Nat` berarti "`x` dan `y` adalah bilangan asli".
  **Jawab: Benar**

2] Apa arti dari pernyataan `∀ x : Prop, x → x`?
a] Ada proposisi `x` sehingga `x → x`.
b] Untuk setiap proposisi `x`, ada proposisi `x → x`.
c] Untuk setiap proposisi `x`, berlaku `x → x`.
d] Ada proposisi `x` sehingga tidak berlaku `x → x`.
**Jawab: c**

3] Diberikan `y : Nat`. Apa arti dari pernyataan `∃ x : Nat, x + y = 0`?
a] Ada bilangan asli `x` sehingga `x + y = 0`.
b] Ada proposisi `x` sehingga `x + y = 0`.
c] Untuk setiap bilangan asli `x`, berlaku `x + y = 0`.
d] Untuk setiap proposisi `x`, berlaku `x + y = 0`.
**Jawab: a**

4] Diberikan definisi suatu fungsi pada Lean sebagai berikut.

```
def pasti_bisa (a : Nat) := ∃ b : Nat, a = b * b
```

Misalkan `x : Nat`. Apa arti dari pernyataan `pasti_bisa x`?
a] `x` adalah bilangan genap.
b] `x` adalah bilangan kuadrat sempurna.
c] `x` adalah bilangan prima.
d] `x` adalah bilangan nonpositif.
**Jawab: b**

5] Manakah kalimat logika yang memiliki arti "untuk setiap proposisi `x` dan `y`, jika `x ∧ y` maka `x`"?
a] `∃ x y : Prop, (x ∧ y) → x`.
b] `∀ x y : Nat, (x ∧ y) → x`.
c] `∀ x y : Prop, x ∧ (y → x)`.
d] `∀ x y : Prop, (x ∧ y) → x`.
**Jawab: d**

6] Manakah kalimat logika yang memiliki arti "ada bilangan asli `x` sehingga `x * x = x + x`"?
a] `∃ x : Nat, x * x = x + x`.
b] `∀ x : Nat, x * x = x + x`.
c] `∃ x : Prop, x * x = x + x`.
d] `∃ x : Type, x * x = x + x`.
**Jawab: a**

7] Manakah kalimat logika yang memiliki arti "untuk setiap proposisi `x`, ada proposisi `y` sehingga `x ↔ y`"?
a] `∃ x : Prop, (∃ y : Prop, x ↔ y)`.
b] `∀ x : Prop, (∀ y : Prop, x ↔ y)`.
c] `∃ x : Prop, (∀ y : Prop, x ↔ y)`.
d] `∀ x : Prop, (∃ y : Prop, x ↔ y)`.
**Jawab: d**

8] Diberikan suatu teorema pada Lean sebagai berikut (amati bahwa buktinya belum lengkap).

```
variable (a : Type)
variable (P : a → Prop)
variable (Q : a → Prop)

example (x : a) (h : Q x) : ∃ y : a, (P y ∨ Q y) := by
  exists x
  exact sorry
```

Manakah sintaks yang dapat digunakan untuk mengganti `sorry` pada bukti yang diberikan agar bukti selesai?
a] `Or.inr x`
b] `Or.inl x`
c] `Or.inr h`.
d] `Or.inl h`.
**Jawab: c**

9] Diberikan suatu teorema pada Lean sebagai berikut (amati bahwa buktinya belum lengkap).

```
example : ∀ (x : Prop), x → x := by
  intro x
  intro hx
  exact sorry
```

Manakah sintaks yang dapat digunakan untuk mengganti `sorry` pada bukti yang diberikan agar bukti selesai?
a] `x`.
b] `exists x`.
c] `hx x`.
d] `hx`.
**Jawab: d**

10] Diberikan suatu teorema pada Lean sebagai berikut (amati bahwa buktinya belum lengkap).

```
example : ∃ (a : Nat), a + 3 = 10 := by
  sorry
```

Manakah sintaks yang dapat digunakan untuk mengganti `sorry` pada bukti yang diberikan agar bukti selesai?
a] `exists 6`.
b] `exists 7`.
c] `exists 8`.
d] `exists 9`.
**Jawab: b**