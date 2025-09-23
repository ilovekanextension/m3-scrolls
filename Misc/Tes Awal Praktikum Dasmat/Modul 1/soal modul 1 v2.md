1] Diberikan suatu teorema pada Lean sebagai berikut.

```
theorem a (b : B) : c := sorry
```

Manakah pernyataan yang benar?
a] `b : B` adalah nama dari teorema tersebut.
b] `c` adalah suatu hipotesis dari teorema tersebut.
c] `a` adalah bukti dari teorema tersebut.
d] Bukti dari teorema tersebut belum diberikan.
**Jawab: d**

2] Diberikan tampilan *tactic state* dalam pengerjaan suatu teorema pada Lean sebagai berikut.

> 1. Tactic State
> 2. $\mathsf{1 \ Goal}$
> 3. $\mathsf{P \ Q \ : \ Prop}$
> 4. $\mathsf{x \ : \ P \to Q}$
> 5. $\mathsf{\vdash \ \neg Q \to \neg P}$

Manakah baris yang menunjukkan *goal* saat ini?
a] Baris 3
b] Baris 4
c] Baris 5
d] *Goal* tidak ditampilkan.
**Jawab: c**

3] Diberikan hipotesis `hp : P` dan `hq : Q`. Sintaks manakah yang dapat digunakan untuk menyelesaikan *goal* `P ∧ Q`?
a] Sintaks `exact hp`.
b] Sintaks `exact ⟨hq, hp⟩`.
c] Sintaks `exact hq`.
d] Sintaks `exact ⟨hp, hq⟩`.
**Jawab: d**

4] Diberikan hipotesis `hp : P` dan `hq : Q`. Sintaks manakah yang dapat digunakan untuk menyelesaikan *goal* `P ∨ Q`?
a] Sintaks `exact Or.inr hp`.
b] Sintaks `exact Or.inl hp`.
c] Sintaks `exact ⟨hp, hq⟩`.
d] Sintaks `exact hp`.
**Jawab: b**

5] Diberikan *goal* `P → Q` dan hipotesis `hq : Q`. Manakah cara pembuktian yang sesuai untuk skenario yang diberikan?
a] Mulai bukti dengan `intro h`, kemudian selesaikan dengan `exact hq`.
b] Mulai bukti dengan `intro h`, kemudian selesaikan dengan `exact h`.
c] Mulai bukti dengan `intro h`, kemudian selesaikan dengan `h`.
d] Mulai bukti dengan `intro h`, kemudian selesaikan dengan `hq`.
**Jawab: a**

6] Diberikan hipotesis `h : P ∧ Q`. Manakah pernyataan yang benar?
a] `exact h.right` dapat digunakan untuk menyelesaikan *goal* `Q`.
b] `exact left h` dapat digunakan untuk menyelesaikan *goal* `P`.
c] `exact h.right h.left` dapat digunakan untuk menyelesaikan *goal* `Q ∧ P`.
d] `exact Or.inr h` dapat digunakan untuk menyelesaikan *goal* `Q`.
**Jawab: a**

7] Diberikan suatu teorema pada Lean sebagai berikut (amati bahwa buktinya belum lengkap).

```
example (P : Prop) : P → (P ∨ P) := by
	intro hp
	sorry
```

Manakah sintaks yang dapat digunakan untuk mengganti `sorry` pada bukti yang diberikan agar bukti selesai?
a] `exact hp`.
b] `exact Or.inr hp`.
c] `exact ⟨hp, hp⟩`.
d] `exact hp.right`.
**Jawab: b**

8] Diberikan suatu teorema pada Lean sebagai berikut (amati bahwa buktinya belum lengkap).

```
example (P : Prop) (h : P → ¬Q) : Q → ¬P := by
	intro hq
	intro hp
	exact (sorry) hq
```

Manakah sintaks yang dapat digunakan untuk mengganti `sorry` pada bukti yang diberikan agar bukti selesai?
a] `h hp`.
b] `hp h`.
c] `h`.
d] `hp`.
**Jawab: a**

9] Diberikan suatu teorema pada Lean sebagai berikut (amati bahwa buktinya belum lengkap).

```
example (P Q : Prop) (h : P ↔ Q) : Q ↔ P := by
	constructor
	. exact sorry1
	. exact sorry2
```

Manakah sintaks yang dapat digunakan untuk mengganti `sorry1` dan `sorry2` berturut-turut pada bukti yang diberikan agar bukti selesai?
a] `h.left` dan `h.right`.
b] `h.right` dan `h.left`.
c] `h.mpr` dan `h.mp`.
d] `h.mp` dan `h.mpr`.
**Jawab: c**

10] Diberikan suatu teorema pada Lean sebagai berikut (amati bahwa buktinya belum lengkap).

```
example (P Q : Prop) (hp : P) : ¬P → Q := by
	intro hnp
	exfalso
	sorry
```

Manakah sintaks yang dapat digunakan untuk mengganti `sorry` berturut-turut pada bukti yang diberikan agar bukti selesai?
a] `exact hp hnp`.
b] `exact apply hnp`.
c] `exact apply hp hnp`.
d] `exact hnp hp`.
**Jawab: d**