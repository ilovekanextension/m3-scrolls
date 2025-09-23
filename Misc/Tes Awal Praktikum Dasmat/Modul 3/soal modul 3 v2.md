1] Untuk setiap pernyataan di bawah, tentukan kebenarannya.
- Jika diberikan semesta `U`, `Set U` adalah tipe dari himpunan dengan anggota-anggota bertipe `U`.
  **Jawab: Benar**
- Jika diberikan dua himpunan `A : Set U` dan `B : Set U`, irisan kedua himpunan ini dinotasikan dengan `A ∩ B`.
  **Jawab: Benar**
- Jika diberikan semesta `U` dan `x : U`, pernyataan `x ∈ ∅` ekuivalen dengan `True`.
  **Jawab: Salah**

2] Diberikan semesta `U`. Manakah pernyataan yang ekuivalen dengan `x ∈ A ∪ B`?
a] `x ∈ A ∧ x ∈ B`.
b] `x ∈ A ∨ x ∈ B`.
c] `x ∈ A → x ∈ B`.
d] `x ∈ A ∨ x ∉ B`.
**Jawab: b**

3] Diberikan `A B : Set U`. Apa arti dari pernyataan `x ∉ A ∩ B`?
a] `x` bukan anggota dari irisan `A` dan `B`.
b] `x` adalah anggota dari irisan `A` dan `B`.
c] `x` bukan anggota dari gabungan `A` dan `B`.
d] `x` adalah anggota dari gabungan `A` dan `B`.
**Jawab: a**

4] Diberikan `A B : Set U`. Apa arti dari pernyataan `Aᶜ ⊆ B`?
a] `A` adalah himpunan bagian dari `B`.
b] `B` adalah himpunan bagian dari komplemen dari `A`.
c] Komplemen dari `A` adalah himpunan bagian dari `B`.
d] Komplemen dari `B` adalah himpunan bagian dari `A`.
**Jawab: c**

5] Diberikan `A : Set U`. Manakah yang **akan selalu** merupakan himpunan kosong?
a] `A ∩ Aᶜ`.
b] `A ∪ Aᶜ`.
c] `A ∪ A`.
d] `A ∩ A`.
**Jawab: a**

6] Diberikan semesta `U`. Himpunan `Set.univ` adalah himpunan dari semua anggota bertipe `U`. Oleh karena itu, setiap elemen bertipe `U` adalah anggota dari `Set.univ`. Manakah pernyataan yang menggambarkan observasi ini?
a] `∀ (x : U), x ∉ Set.univ`.
b] `∃ (x : U), x ∉ Set.univ`.
c] `∃ (x : U), x ∈ Set.univ`.
d] `∀ (x : U), x ∈ Set.univ`.
**Jawab: d**

7] Diberikan semesta `U` dan himpunan `A : Set U`. Manakah pernyataan di bawah ini yang **selalu benar**?
a] `A ⊆ ∅`.
b] `A = ∅`.
c] `Set.univ ⊆ A`.
d] `A ⊆ A`.
**Jawab: d**

8] Diberikan suatu teorema pada Lean sebagai berikut (amati bahwa buktinya belum lengkap).

```
example (U : Type) (A : Set U) : A ⊆ A := by
	intro x
	intro hx
	sorry
```

Manakah sintaks yang dapat digunakan untuk mengganti `sorry` pada bukti yang diberikan agar bukti selesai?
a] `exact x`.
b] `exact hx`.
c] `contradiction`.
d] `True`.
**Jawab: b**

9] Diberikan suatu teorema pada Lean sebagai berikut (amati bahwa buktinya belum lengkap).

```
example (U : Type) (A : Set U) : (∅ : Set U) ⊆ A := by
	intro x
	intro hx
	sorry
```

Manakah sintaks yang dapat digunakan untuk mengganti `sorry` pada bukti yang diberikan agar bukti selesai?
a] `exact hx`.
b] `trivial`.
c] `contradiction`.
d] `exact False`.
**Jawab: c**

10] Diberikan suatu teorema pada Lean sebagai berikut (amati bahwa buktinya belum lengkap).

```
example (U : Type) (A B : Set U) : A ∩ B ⊆ A := by
	intro x
	intro hx
	exact sorry
```

Manakah sintaks yang dapat digunakan untuk mengganti `sorry` pada bukti yang diberikan agar bukti selesai?
a] `hx.right`.
b] `hx.left`.
c] `hx`.
d] `hx.A`.
**Jawab: b**