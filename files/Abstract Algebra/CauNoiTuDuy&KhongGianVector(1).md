# LỘ TRÌNH TOÀN DIỆN: TỪ LỚP 9 ĐẾN NĂNG LỰC CHUYÊN GIA
## Đại số đa tuyến tính (Multilinear Algebra) & Lý thuyết biểu diễn (Representation Theory)

---

## LỜI NÓI ĐẦU

Tài liệu này gồm hai phần:

- **Phần A** — bản đồ tổng thể của *toàn bộ* con đường, từ nền tảng lớp 9 đến trình độ có thể đọc hiểu và sử dụng thành thạo hai lĩnh vực trên. Đây là khung chương trình để giáo sư lên kế hoạch giảng dạy nhiều năm.
- **Phần B, C** — nội dung thật, viết đầy đủ, có định nghĩa – định lý – chứng minh – ví dụ – bài tập, cho hai mắt xích đầu tiên: *Cầu nối tư duy* và *Không gian vector*. Đây không phải tóm tắt hay giới thiệu sơ lược — đây là giáo trình có thể dạy trực tiếp.

Nguyên tắc xuyên suốt: **không có định lý nào được chấp nhận mà không có chứng minh, không có khái niệm nào được dùng trước khi được định nghĩa.**

---

## PHẦN A — BẢN ĐỒ TỔNG THỂ

### Tại sao phải đi đúng thứ tự này

Lý thuyết biểu diễn nhóm, ở bản chất, nghiên cứu **module trên vành nhóm** $F[G]$. Muốn hiểu "module" phải hiểu "vành" và "nhóm" trước. Đại số đa tuyến tính, ở bản chất, nghiên cứu **ánh xạ đa tuyến tính** và các cấu trúc sinh ra từ chúng (tích tenxơ, đại số ngoài). Muốn định nghĩa tích tenxơ một cách chặt chẽ (bằng *tính chất phổ dụng* — universal property) cần nắm vững không gian vector, ánh xạ tuyến tính, và không gian đối ngẫu ở mức tiên đề. Không có nền tảng đó, "tenxơ" chỉ là một mảng số có chỉ số — đúng nhưng nông, và sẽ sụp đổ ngay khi gặp bài toán không phải là $\mathbb{R}^n$ với cơ sở chuẩn.

### Bảng tổng quan 6 giai đoạn

| Giai đoạn | Nội dung cốt lõi | Vì sao bắt buộc | Thời lượng ước tính |
|---|---|---|---|
| **0. Cầu nối tư duy** | Logic mệnh đề, tập hợp, ánh xạ, phương pháp chứng minh, số phức | Đây là *ngôn ngữ* viết nên mọi định nghĩa phía sau | 1–2 tháng |
| **1. Đại số tuyến tính (tiên đề)** | Trường, không gian vector, ánh xạ tuyến tính, không gian đối ngẫu, dạng song tuyến tính, tích trong, trị riêng | Là "vật liệu thô" mà đại số đa tuyến tính mở rộng ra | 6–9 tháng |
| **2. Đại số trừu tượng** | Nhóm, nhóm con/thương, đồng cấu, tác động nhóm, vành, ideal, module | Biểu diễn nhóm = module trên $F[G]$. Không có mắt xích này, "biểu diễn" không có nghĩa | 8–12 tháng |
| **3. Đại số đa tuyến tính** | Ánh xạ đa tuyến tính, tích tenxơ, đại số tenxơ, đại số đối xứng, đại số ngoài | Đây là đối tượng chính thứ nhất | 4–6 tháng |
| **4. Lý thuyết biểu diễn** | Biểu diễn nhóm hữu hạn, Bổ đề Schur, Định lý Maschke, lý thuyết ký tự, biểu diễn cảm sinh | Đây là đối tượng chính thứ hai | 6–9 tháng |
| **5. Hợp nhất & chuyên sâu** | Đối ngẫu Schur–Weyl, biểu diễn của $GL(V)$ trên $\mathrm{Sym}(V)$ và $\Lambda(V)$, ứng dụng vật lý/khoa học dữ liệu | Đây là nơi hai lĩnh vực *hợp nhất* — dấu hiệu thật sự của "chuyên gia" | 6–12+ tháng |

**Tổng: khoảng 2.5 – 4 năm**, với điều kiện học liên tục, có người hướng dẫn, và — quan trọng nhất — **tự làm bài tập, tự viết lại chứng minh**, không chỉ đọc.

Sau khi hoàn thành Giai đoạn 5, học sinh ở trình độ tương đương sinh viên cao học năm nhất chuyên ngành đại số/toán-lý — đủ để đọc paper nghiên cứu và áp dụng thành thạo. Mức "chuyên gia" theo nghĩa nghiên cứu độc lập (tự tạo ra định lý mới) đòi hỏi thêm giai đoạn làm nghiên cứu thật sự dưới một người hướng dẫn — điều này đúng với mọi ngành khoa học, không riêng gì hai lĩnh vực này.

### Chi tiết từng giai đoạn

**Giai đoạn 0 — Cầu nối tư duy**
Logic mệnh đề & lượng từ · Tập hợp & các phép toán · Quan hệ, ánh xạ, đơn/toàn/song ánh · Quy nạp toán học & phản chứng · Số phức và căn bậc $n$ của đơn vị (sẽ quay lại ở biểu diễn của nhóm cyclic).

**Giai đoạn 1 — Đại số tuyến tính tiên đề**
Trường · Không gian vector, không gian con · Độc lập tuyến tính, cơ sở, số chiều · Ánh xạ tuyến tính, ma trận biểu diễn, hạt nhân–ảnh · Định lý hạng–số chiều (rank–nullity) · Định thức (xây dựng qua dạng đa tuyến tính thay phiên — *cầu nối trực tiếp* sang đại số ngoài sau này) · Trị riêng, vector riêng, chéo hóa · **Không gian đối ngẫu $V^*$** (bắt buộc, vì tenxơ hiệp biến/phản biến được định nghĩa qua $V$ và $V^*$) · Dạng song tuyến tính, dạng toàn phương · Không gian tích trong, trực giao hóa Gram–Schmidt, định lý phổ.

*Tài liệu tham khảo:* Sheldon Axler, *Linear Algebra Done Right*; Hoffman & Kunze, *Linear Algebra*.

**Giai đoạn 2 — Đại số trừu tượng**
Nhóm: định nghĩa, nhóm con, định lý Lagrange, nhóm thương, đồng cấu, định lý đẳng cấu · Tác động nhóm lên tập hợp (group action) — nền tảng trực tiếp của biểu diễn · Nhóm hoán vị $S_n$ · Vành, ideal, vành thương · Module trên vành (tổng quát hóa không gian vector — cần thiết vì $F[G]$-module chính là "biểu diễn").

*Tài liệu tham khảo:* Dummit & Foote, *Abstract Algebra*; Michael Artin, *Algebra*.

**Giai đoạn 3 — Đại số đa tuyến tính**
Ánh xạ đa tuyến tính · Tích tenxơ $V \otimes W$ (định nghĩa bằng tính chất phổ dụng) · Đại số tenxơ $T(V) = \bigoplus_k V^{\otimes k}$ · Đại số đối xứng $\mathrm{Sym}(V)$ · Đại số ngoài $\Lambda(V)$ và tích ngoài (wedge product) · Tenxơ hiệp biến/phản biến, quy tắc đổi chỉ số · Định thức như phần tử của $\Lambda^n(V)$, dạng thể tích.

*Tài liệu tham khảo:* Werner Greub, *Multilinear Algebra*; Steven Roman, *Advanced Linear Algebra*.

**Giai đoạn 4 — Lý thuyết biểu diễn**
Biểu diễn của nhóm hữu hạn trên không gian vector · Biểu diễn bất khả quy, biểu diễn khả quy hoàn toàn · **Bổ đề Schur** · **Định lý Maschke** · Lý thuyết ký tự, tính trực giao của ký tự, bảng ký tự · Biểu diễn cảm sinh, định lý tương hỗ Frobenius · Biểu diễn của $S_n$ (giới thiệu bảng Young).

*Tài liệu tham khảo:* Jean-Pierre Serre, *Linear Representations of Finite Groups*; Fulton & Harris, *Representation Theory: A First Course*.

**Giai đoạn 5 — Hợp nhất & chuyên sâu**
Đối ngẫu Schur–Weyl (nhóm $GL(V)$ và $S_n$ cùng tác động lên $V^{\otimes n}$ — điểm giao thoa thật sự của hai lĩnh vực) · Biểu diễn trên $\mathrm{Sym}^k(V)$, $\Lambda^k(V)$ · Ứng dụng: tenxơ metric trong thuyết tương đối, spin trong cơ học lượng tử, phân tích tenxơ (tensor decomposition) trong khoa học dữ liệu.

---

## PHẦN B — GIAI ĐOẠN 0: CẦU NỐI TƯ DUY (nội dung đầy đủ)

### 0.1 Mệnh đề và lượng từ

Một **mệnh đề** là một câu khẳng định có giá trị chân lý xác định: đúng hoặc sai, không cả hai. Các phép nối: $\neg P$ (phủ định), $P \wedge Q$ (và), $P \vee Q$ (hoặc), $P \Rightarrow Q$ (kéo theo), $P \Leftrightarrow Q$ (tương đương).

Điều **quan trọng nhất** cần nắm chắc là phủ định của mệnh đề có lượng từ:
$$\neg(\forall x,\, P(x)) \iff \exists x,\, \neg P(x)$$
$$\neg(\exists x,\, P(x)) \iff \forall x,\, \neg P(x)$$

Đây không phải "quy tắc học vẹt" — nó là lý do vì sao, để chứng minh "không tồn tại $x$ thỏa mãn $P(x)$", ta chứng minh "$P(x)$ sai với mọi $x$".

### 0.2 Tập hợp

Tập hợp là một khái niệm nguyên thủy (không định nghĩa lại được bằng khái niệm đơn giản hơn), chỉ mô tả bằng tiên đề. Ta dùng: $x \in A$ (thuộc), $A \subseteq B$ (tập con: $\forall x, x\in A \Rightarrow x \in B$), $A \cup B$, $A \cap B$, $A \setminus B$, tập rỗng $\varnothing$, tập lũy thừa $2^A$ (tập hợp mọi tập con của $A$), tích Descartes $A \times B = \{(a,b) : a\in A, b\in B\}$.

**Định lý 0.2.1.** Nếu $|A| = n$ (hữu hạn) thì $|2^A| = 2^n$.

*Chứng minh (quy nạp theo $n$).* Với $n=0$: $A = \varnothing$, $2^A = \{\varnothing\}$, có $1 = 2^0$ phần tử. Giả sử đúng với $n=k$. Xét $|A| = k+1$, chọn $a \in A$, đặt $A' = A \setminus \{a\}$ nên $|A'| = k$. Mỗi tập con của $A$ hoặc chứa $a$ hoặc không: các tập con không chứa $a$ chính là các tập con của $A'$ (có $2^k$ theo giả thiết quy nạp); các tập con chứa $a$ có dạng $S \cup \{a\}$ với $S$ là tập con của $A'$ (cũng có $2^k$, và tương ứng $S \mapsto S\cup\{a\}$ là song ánh). Hai loại này rời nhau, nên $|2^A| = 2^k + 2^k = 2^{k+1}$. $\blacksquare$

### 0.3 Ánh xạ

Một **ánh xạ** $f: A \to B$ là một quy tắc gán mỗi $a \in A$ với đúng một phần tử $f(a) \in B$ — chính xác hơn, $f$ là một tập con của $A \times B$ sao cho với mỗi $a \in A$, tồn tại *duy nhất* $b \in B$ với $(a,b) \in f$.

- $f$ **đơn ánh** (injective) nếu $f(a_1) = f(a_2) \Rightarrow a_1 = a_2$.
- $f$ **toàn ánh** (surjective) nếu $\forall b \in B, \exists a \in A: f(a) = b$.
- $f$ **song ánh** (bijective) nếu vừa đơn ánh vừa toàn ánh.

**Định lý 0.3.1.** $f: A \to B$ có ánh xạ ngược $f^{-1}: B \to A$ (thỏa $f^{-1}(f(a))=a$ và $f(f^{-1}(b))=b$) khi và chỉ khi $f$ song ánh.

*Chứng minh.*
($\Rightarrow$) Nếu $f^{-1}$ tồn tại: $f$ đơn ánh vì $f(a_1)=f(a_2) \Rightarrow f^{-1}(f(a_1)) = f^{-1}(f(a_2)) \Rightarrow a_1=a_2$. $f$ toàn ánh vì với mọi $b\in B$, $a := f^{-1}(b)$ thỏa $f(a) = b$.

($\Leftarrow$) Nếu $f$ song ánh: với mỗi $b \in B$, do toàn ánh, tồn tại $a\in A$ với $f(a)=b$; do đơn ánh, $a$ này là duy nhất. Định nghĩa $f^{-1}(b) := a$. Đây là một ánh xạ hợp lệ (mỗi $b$ ứng đúng một $a$) và theo cách xây dựng, thỏa hai đẳng thức trên. $\blacksquare$

### 0.4 Phương pháp chứng minh

**Quy nạp toán học.** Để chứng minh $P(n)$ đúng với mọi $n \geq n_0$: (i) chứng minh $P(n_0)$ đúng (cơ sở); (ii) chứng minh $P(k) \Rightarrow P(k+1)$ với mọi $k \geq n_0$ (bước quy nạp). Nguyên lý này *không phải* một định lý cần chứng minh thêm — nó là một tiên đề của tập số tự nhiên (tiên đề Peano thứ 5).

**Phản chứng.** Để chứng minh $P$, giả sử $\neg P$ đúng và suy ra một mâu thuẫn (một mệnh đề vừa đúng vừa sai).

*Ví dụ kinh điển:* $\sqrt{2}$ là số vô tỉ. Giả sử ngược lại, $\sqrt{2} = p/q$ với $p,q$ nguyên, $\gcd(p,q)=1$. Khi đó $p^2 = 2q^2$, nên $p^2$ chẵn, suy ra $p$ chẵn (vì nếu $p$ lẻ thì $p^2$ lẻ), viết $p=2r$. Thay vào: $4r^2 = 2q^2 \Rightarrow q^2 = 2r^2$, suy ra $q$ cũng chẵn. Nhưng $p,q$ cùng chẵn mâu thuẫn với $\gcd(p,q)=1$. $\blacksquare$

### 0.5 Từ số hữu tỉ đến số phức: khái niệm Trường (giới thiệu sớm)

Một **trường** (field) $F$ là một tập hợp có hai phép toán $+, \times$ sao cho $(F,+)$ là nhóm giao hoán (có phần tử trung hòa $0$), $(F\setminus\{0\}, \times)$ là nhóm giao hoán (có phần tử đơn vị $1$), và phép nhân phân phối với phép cộng: $a(b+c)=ab+ac$.

$\mathbb{Q}, \mathbb{R}, \mathbb{C}$ đều là trường. $\mathbb{Z}$ **không phải** trường (số nguyên khác $\pm 1$ không có nghịch đảo nhân trong $\mathbb{Z}$).

**Số phức:** $\mathbb{C} = \{a + bi : a, b \in \mathbb{R}\}$, với $i^2 = -1$. Dạng lượng giác: $z = r(\cos\theta + i\sin\theta)$, và công thức Euler $e^{i\theta} = \cos\theta + i\sin\theta$ cho $z = re^{i\theta}$.

**Công thức De Moivre:** $(\cos\theta + i \sin\theta)^n = \cos(n\theta) + i\sin(n\theta)$.

*Chứng minh (quy nạp theo $n \geq 1$).* Cơ sở $n=1$: hiển nhiên. Bước quy nạp: giả sử đúng với $n=k$. Khi đó
$$(\cos\theta+i\sin\theta)^{k+1} = (\cos\theta+i\sin\theta)^k(\cos\theta+i\sin\theta) = (\cos k\theta + i \sin k\theta)(\cos\theta+i\sin\theta).$$
Nhân ra và dùng công thức cộng lượng giác $\cos(A+B) = \cos A\cos B - \sin A \sin B$, $\sin(A+B)=\sin A \cos B + \cos A \sin B$, ta được đúng $\cos((k+1)\theta) + i\sin((k+1)\theta)$. $\blacksquare$

Hệ quả: nghiệm của $x^n = 1$ trong $\mathbb{C}$ là $n$ **căn bậc $n$ của đơn vị** $e^{2\pi i k/n}$, $k=0,\ldots,n-1$ — tập hợp này, với phép nhân, tạo thành một **nhóm cyclic** cấp $n$. (Ghi nhớ điều này — nó sẽ xuất hiện lại nguyên vẹn khi học biểu diễn của nhóm cyclic ở Giai đoạn 4.)

### Bài tập Giai đoạn 0

1. Viết phủ định của mệnh đề: "Với mọi $\varepsilon>0$, tồn tại $N$ sao cho với mọi $n>N$, $|a_n - L| < \varepsilon$."
2. Chứng minh bằng quy nạp: $1^3+2^3+\cdots+n^3 = \left(\frac{n(n+1)}{2}\right)^2$.
3. Chứng minh $f: \mathbb{R}\to\mathbb{R}, f(x)=x^3$ là song ánh. Tìm $f^{-1}$.
4. Dùng phản chứng, chứng minh có vô hạn số nguyên tố.
5. Tìm tất cả nghiệm của $x^4=1$ trong $\mathbb{C}$, biểu diễn trên mặt phẳng phức, và kiểm tra chúng tạo thành nhóm dưới phép nhân.

---

## PHẦN C — CHƯƠNG 1: KHÔNG GIAN VECTOR (mở đầu Giai đoạn 1)

### 1.1 Trường — nhắc lại chính xác

*(đã định nghĩa ở 0.5 — đây là "thế giới vô hướng" mà không gian vector sẽ được xây trên đó)*

### 1.2 Định nghĩa không gian vector

Cho $F$ là một trường. Một **không gian vector trên $F$** là một tập hợp $V$ cùng hai phép toán:
- phép cộng $V \times V \to V$, $(u,v) \mapsto u+v$
- phép nhân vô hướng $F \times V \to V$, $(a,v) \mapsto av$

thỏa mãn 8 tiên đề sau, với mọi $u,v,w \in V$ và $a,b \in F$:

1. $(u+v)+w = u+(v+w)$ (kết hợp)
2. $u+v = v+u$ (giao hoán)
3. Tồn tại $0_V \in V$ sao cho $v + 0_V = v$ với mọi $v$ (phần tử trung hòa)
4. Với mỗi $v$, tồn tại $-v$ sao cho $v+(-v)=0_V$ (phần tử đối)
5. $1_F \cdot v = v$
6. $a(bv) = (ab)v$
7. $a(u+v) = au+av$
8. $(a+b)v = av+bv$

Các phần tử của $V$ gọi là **vector**, các phần tử của $F$ gọi là **vô hướng** (scalar).

### 1.3 Ví dụ

- $F^n = \{(a_1,\ldots,a_n) : a_i \in F\}$, với cộng và nhân vô hướng theo từng tọa độ.
- $M_{m\times n}(F)$: ma trận cỡ $m\times n$ trên $F$.
- $F[x]$: đa thức một biến hệ số trong $F$.
- $F[x]_{\leq n}$: đa thức bậc $\leq n$.
- $\mathrm{Func}(S,F) = \{f : S \to F\}$ với mọi tập $S$: cộng và nhân vô hướng theo điểm.

**Điều cần nhấn mạnh với học sinh:** "vector" ở đây *không nhất thiết* là mũi tên có hướng trong không gian — nó là *bất kỳ đối tượng nào* thỏa 8 tiên đề trên. Đa thức là vector. Ma trận là vector. Đây là bước nhảy tư duy quan trọng nhất của chương này.

### 1.4 Hệ quả cơ bản (với chứng minh đầy đủ)

**Định lý 1.4.1.** $0_F \cdot v = 0_V$ với mọi $v \in V$.

*Chứng minh.* Đặt $w = 0_F \cdot v$. Ta có $w = (0_F+0_F)v = 0_F v + 0_F v = w+w$ (dùng tiên đề 8). Cộng $-w$ vào hai vế: $-w+w = -w+(w+w) = (-w+w)+w$ (tiên đề 1), tức $0_V = 0_V + w = w$. Vậy $w=0_V$. $\blacksquare$

**Định lý 1.4.2.** $a\cdot 0_V = 0_V$ với mọi $a \in F$.

*Chứng minh.* Tương tự: $a\cdot 0_V = a(0_V+0_V) = a\cdot0_V + a\cdot 0_V$ (tiên đề 7), và cùng lập luận cộng phần tử đối như trên suy ra $a\cdot 0_V = 0_V$. $\blacksquare$

**Định lý 1.4.3.** $(-1_F)\cdot v = -v$.

*Chứng minh.* $v + (-1_F)v = 1_F v + (-1_F)v = (1_F + (-1_F))v = 0_F \cdot v = 0_V$ (dùng tiên đề 8, 5, và Định lý 1.4.1). Vì phần tử đối trong nhóm cộng là duy nhất, $(-1_F)v = -v$. $\blacksquare$

**Định lý 1.4.4 (Không có ước của không).** Nếu $av = 0_V$ thì $a=0_F$ hoặc $v=0_V$.

*Chứng minh.* Giả sử $a \neq 0_F$. Vì $F$ là trường, $a$ khả nghịch. Khi đó $v = 1_F v = (a^{-1}a)v = a^{-1}(av) = a^{-1}\cdot 0_V = 0_V$ (tiên đề 6, 5, và Định lý 1.4.2). $\blacksquare$

### 1.5 Không gian con

Một tập con $W \subseteq V$ là **không gian con** nếu bản thân $W$, với phép toán kế thừa từ $V$, cũng là một không gian vector.

**Định lý 1.5.1 (Tiêu chuẩn không gian con).** $W \subseteq V$ khác rỗng là không gian con của $V$ khi và chỉ khi:
$$\forall u,v \in W,\ \forall a \in F: \quad au + v \in W.$$

*Chứng minh.*
($\Rightarrow$) Hiển nhiên nếu $W$ đóng kín dưới phép cộng và nhân vô hướng.

($\Leftarrow$) Giả sử điều kiện trên đúng.
- Lấy $u=v \in W$ bất kỳ, $a = -1_F$: ta có $-v + v = 0_V \in W$. Vậy $0_V \in W$.
- Đóng kín cộng: lấy $a=1_F$: $u+v \in W$ với mọi $u,v \in W$.
- Đóng kín nhân vô hướng: với $a\in F$, $u \in W$, dùng $v = 0_V \in W$ (đã có ở trên): $au + 0_V = au \in W$.

$W$ chứa $0_V$, đóng kín dưới cả hai phép toán; các tiên đề còn lại (kết hợp, giao hoán, phân phối,...) đúng cho *mọi* phần tử của $V$ nên tự động đúng cho các phần tử của $W \subseteq V$. Vậy $W$ là không gian vector, tức không gian con. $\blacksquare$

*Ví dụ:* Tập nghiệm của hệ phương trình tuyến tính thuần nhất $Ax = 0$ là không gian con của $F^n$ — trực tiếp từ Định lý 1.5.1, vì nếu $Au=0, Av=0$ thì $A(au+v) = aAu + Av = 0$.

### 1.6 Tổ hợp tuyến tính, span, độc lập tuyến tính

Cho $S = \{v_1,\ldots,v_k\} \subseteq V$. Một **tổ hợp tuyến tính** của $S$ là biểu thức $a_1v_1+\cdots+a_kv_k$ với $a_i \in F$. Tập tất cả tổ hợp tuyến tính gọi là $\mathrm{span}(S)$.

**Định lý 1.6.1.** $\mathrm{span}(S)$ là không gian con nhỏ nhất của $V$ chứa $S$.

*Chứng minh.* $\mathrm{span}(S)$ là không gian con: nếu $u = \sum a_iv_i$, $w=\sum b_iv_i \in \mathrm{span}(S)$ thì $cu+w = \sum(ca_i+b_i)v_i \in \mathrm{span}(S)$ (Định lý 1.5.1). Rõ ràng $S \subseteq \mathrm{span}(S)$ (lấy hệ số $1$ cho một vector, $0$ cho các vector còn lại). Nếu $W$ là không gian con bất kỳ chứa $S$, thì do đóng kín dưới tổ hợp tuyến tính, $W$ phải chứa mọi tổ hợp tuyến tính của $S$, tức $\mathrm{span}(S) \subseteq W$. $\blacksquare$

$S$ được gọi là **độc lập tuyến tính** nếu: $a_1v_1+\cdots+a_kv_k = 0_V \Rightarrow a_1=\cdots=a_k=0_F$. Ngược lại, $S$ **phụ thuộc tuyến tính**.

### 1.7 Cơ sở và số chiều

$S \subseteq V$ là một **cơ sở** nếu $S$ độc lập tuyến tính và $\mathrm{span}(S) = V$.

**Định lý 1.7.1 (Bổ đề trao đổi Steinitz).** Nếu $\{v_1,\ldots,v_n\}$ sinh ra $V$ và $\{w_1,\ldots,w_m\}$ độc lập tuyến tính trong $V$, thì $m \leq n$.

*Chứng minh (quy nạp).* Ta chứng minh mệnh đề mạnh hơn: với mỗi $k=0,1,\ldots,m$, có thể sắp lại thứ tự các $v_i$ sao cho $\{w_1,\ldots,w_k,v_{k+1},\ldots,v_n\}$ vẫn sinh ra $V$ (và $k \leq n$).

*Cơ sở* $k=0$: đúng theo giả thiết.

*Bước quy nạp:* giả sử đúng với $k<m$. Vì $\{w_1,\ldots,w_k,v_{k+1},\ldots,v_n\}$ sinh ra $V$, ta viết
$$w_{k+1} = \sum_{i=1}^{k} b_i w_i + \sum_{j=k+1}^{n} c_j v_j.$$
Nếu tất cả $c_j = 0$ thì $w_{k+1}$ là tổ hợp tuyến tính của $w_1,\ldots,w_k$, mâu thuẫn với tính độc lập tuyến tính của $\{w_1,\ldots,w_m\}$ (đẳng thức $w_{k+1} - \sum b_iw_i = 0$ có hệ số của $w_{k+1}$ bằng $1 \neq 0$). Vậy tồn tại $j \geq k+1$ với $c_j \neq 0$ — điều này *đồng thời chứng tỏ* $k+1 \leq n$ (phải có ít nhất một $v_j$ với $j\geq k+1$ để chọn). Sắp lại để $j = k+1$, giải ra:
$$v_{k+1} = \frac{1}{c_{k+1}}\Big(w_{k+1} - \sum_{i=1}^k b_iw_i - \sum_{j=k+2}^n c_jv_j\Big).$$
Do đó $\{w_1,\ldots,w_{k+1},v_{k+2},\ldots,v_n\}$ sinh ra mọi thứ mà tập cũ sinh ra (vì $v_{k+1}$ đã được biểu diễn qua tập mới), tức sinh ra $V$. Theo nguyên lý quy nạp, mệnh đề đúng với $k=m$: cụ thể $m \leq n$. $\blacksquare$

**Hệ quả 1.7.2.** Nếu $V$ có một cơ sở hữu hạn, thì mọi cơ sở của $V$ đều có cùng số phần tử.

*Chứng minh.* Nếu $\{v_1,\ldots,v_n\}$ và $\{w_1,\ldots,w_m\}$ đều là cơ sở: áp dụng Định lý 1.7.1 hai chiều (mỗi cơ sở vừa là tập sinh vừa là tập độc lập) được cả $m\leq n$ và $n\leq m$, vậy $m=n$. $\blacksquare$

Số phần tử chung đó gọi là **số chiều** $\dim(V)$.

**Định lý 1.7.3 (Mở rộng cơ sở).** Mọi tập độc lập tuyến tính trong không gian $V$ hữu hạn chiều đều có thể mở rộng thành một cơ sở của $V$.

*Ý tưởng chứng minh:* nếu tập độc lập tuyến tính $S$ chưa sinh ra $V$, tồn tại $v \notin \mathrm{span}(S)$; khi đó $S \cup \{v\}$ vẫn độc lập tuyến tính (nếu không, $v$ sẽ biểu diễn được qua $S$, mâu thuẫn). Lặp lại quá trình này; theo Định lý 1.7.1, quá trình phải dừng sau tối đa $\dim(V)$ bước, khi đó tập thu được sinh ra $V$. $\blacksquare$

### Bài tập Chương 1

1. Chứng minh $F[x]_{\leq n}$ (đa thức bậc $\leq n$) là không gian vector với $\dim = n+1$, cơ sở chuẩn $\{1,x,x^2,\ldots,x^n\}$.
2. Cho $V = F^3$. Xét $W = \{(x,y,z) : x+y+z=0\}$. Chứng minh $W$ là không gian con bằng Định lý 1.5.1, tìm một cơ sở của $W$ và tính $\dim W$.
3. Chứng minh: nếu $\{v_1,v_2,v_3\}$ độc lập tuyến tính thì $\{v_1, v_1+v_2, v_1+v_2+v_3\}$ cũng độc lập tuyến tính.
4. Tại sao trong Định lý 1.4.4, giả thiết "$F$ là trường" (không chỉ là vành) lại thiết yếu? (Gợi ý: thử $F = \mathbb{Z}$, xét không gian $\mathbb{Z}$-module $\mathbb{Z}/6\mathbb{Z}$ và phần tử $2 \cdot 3 = 6 \equiv 0$.)
5. Chứng minh chi tiết Định lý 1.7.3 bằng quy nạp mạnh, viết rõ từng bước "vì sao $S\cup\{v\}$ độc lập tuyến tính".

---

## PHẦN D — DÙNG LỘ TRÌNH NÀY NHƯ THẾ NÀO

**Về sư phạm:** đọc thôi không tạo ra hiểu. Sau mỗi định lý ở trên, nên yêu cầu học sinh **gấp sách lại và tự viết lại chứng minh bằng lời của mình** trước khi xem lại. Đây là điểm khác biệt duy nhất giữa "học sinh nhớ định lý" và "học sinh hiểu đại số tuyến tính".

**Về nhịp độ:** đừng vội chuyển giai đoạn khi học sinh chưa tự làm được các bài tập dạng "chứng minh $X$ là/không là không gian con", "chứng minh tập này độc lập/phụ thuộc tuyến tính" một cách trôi chảy, không cần gợi ý.

**Bước tiếp theo:** nếu giáo sư muốn, tôi có thể viết tiếp theo đúng phong cách này:
- **Chương 2:** Ánh xạ tuyến tính, ma trận biểu diễn, định lý hạng–số chiều
- **Chương 3:** Không gian đối ngẫu $V^*$ — bản lề trực tiếp dẫn sang đại số đa tuyến tính
- **Chương 4:** Định thức xây dựng như dạng đa tuyến tính thay phiên (đây chính là hạt giống đầu tiên của đại số ngoài)

Mỗi chương sẽ được viết với cùng mức độ chặt chẽ như trên.
