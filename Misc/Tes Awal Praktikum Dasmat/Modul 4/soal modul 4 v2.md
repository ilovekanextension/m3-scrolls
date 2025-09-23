1] Untuk setiap pernyataan di bawah ini, tentukan kebenarannya.
- Pada tipe bilangan asli `Nat`, fungsi `succ : Nat → Nat` adalah fungsi yang memetakan bilangan asli `n : Nat` ke bilangan `n + 1`.
  **Jawab: Benar**
- Tipe bilangan asli `Nat` adalah tipe induktif. Artinya, untuk membuktikan kebenaran dari suatu pernyataan `P` untuk semua bilangan asli pada `Nat`, kita hanya perlu membuktikan kebenaran `P(0)` dan kebenaran `P(n) → P(succ n)` untuk setiap `n : Nat`.
  **Jawab : Benar**

2] Diberikan `m n : Nat`. Manakah di bawah ini yang sesuai untuk dijadikan sebagai hasil dari `m + succ n`?
a] `succ m`.
b] `succ n`.
c] `succ (m + n)`.
d] `succ m + succ n`.
**Jawab: c**

3] Diberikan `m n : Nat`. Manakah di bawah ini yang sesuai untuk dijadikan sebagai hasil dari `m * succ n`?
a] `m * n + m`.
b] `succ (m * n)`.
c] `m * n`.
d] `m + n`.
**Jawab: a**

4] Misalkan kita ingin mendefinisikan suatu operasi perpangkatan `pow : Nat → Nat → Nat` pada `Nat` (jadi `pow m n` berarti $m^n$). Secara intuitif, definisi induktif untuk perpangkatan adalah sebagai berikut:
- Untuk setiap `n : Nat`, $n^0=1$.
- Untuk setiap `m n : Nat`, $m^{n+1}=m^n \times m$.

Berdasarkan definisi ini, manakah di bawah ini yang sesuai untuk dijadikan sebagai hasil dari `pow m 0`?
a] `pow m m`.
b] `m`.
c] `0`.
d] `1`.
**Jawab: d**

5] Untuk membuktikan suatu pernyataan tentang `Nat` dalam variabel `n`, dapat dilakukan induksi dengan menggunakan rangkaian *tactic* berikut.

```
induction' n with k ih
. sorry1
. sorry2
```

Manakah pernyataan di bawah ini yang benar?
a] Pada tahap induksi, nama dari hipotesis induksi yang digunakan adalah `k`.
b] Pada tahap induksi, variabel yang akan digunakan adalah `n`.
c] `sorry2` perlu diganti dengan bukti untuk kasus dasar (ketika `k = 0`).
d] `sorry1` perlu diganti dengan bukti untuk kasus dasar (ketika `k = 0`).
**Jawab: d**

