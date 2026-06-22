
(vietnamese)

**Authors:** Hung Dinh Phu Dang  

**Date:** 17-18-22, June 2026  

Ý tôi muốn nói là phải giải quyết được bài toán bên dưới một cách cực kỳ "thanh lịch" thông qua việc tạo ra một nền tảng không gian toán học mới (Cách giải quyết thanh lịch nhất lịch sử ?) :

===

Core Research Question :

Rather than asking "How do we compute N scalar answers from N expressions as fast as possible?", we propose asking: "Why do we need scalar outputs when relational structure and total orderings between expressions suffice?"

Primary Hypothesis: ALL contemporary important problems do not fundamentally require scalar decomposition. (If it's considered mandatory to have scalars, then it's an illusion.)

Proposed Framework :

Central Idea :

Construct a mathematically rigorous formal system where:

N symbolic expressions maintain structural integrity (no decomposition into scalars)

Automatic extraction of relational structure that corresponds bijectively to scalar relationships

Computational cost: far superior to "O(n)" (Reality goes beyond)  scalar computation (traditional systems) ;  NOTE : In essence, **the traditional "processing" method doesn't have** a complexity of **O(N)**, however I'm talking about **"computation"**;

Key Properties Required :

Comparability: Any two arbitrary expressions must be comparable using {<, >, =}

Distance metric: Define a "distance" or "gap" between expressions analogous to scalar spacing

Decidability: Computable comparisons with polynomial-time bounds

Decidability: Rational trade-offs preventing theoretical vacuousness

The Preservation Advantage :

By avoiding expression-to-scalar decomposition, we retain structural information about the original expressions. This preserved structure may enable deeper analysis of expression relationships and properties.


Computational Trade-Off :

We propose exchanging generality for decidability and efficiency:

Input Restriction:

N expressions containing only :

Basic arithmetic operations: {+, −, ×, ÷} (Richardson's theorem)

Real numbers with finite precision

Exclusions: Transcendental functions (sin, exp, log, etc.)

The Fundamental Question :

Current Approach

Expressions → Computation → Scalar values

Proposed Approach

Expressions → Relational Structure (preserving all ordering/distance properties of scalar equivalents) → Direct analysis at reduced computational cost

The Key Insight :

Rather than ask "To what extent can this method replace scalars?", we should ask: "Do meaningful contemporary applications actually gain any advantage from scalar decomposition when relational structure & "distance" is properly formalized?"



In other words: when relational properties, total orderings, and distance metrics are correctly developed, don't scalars become computationally redundant?

Challenges & Requirements :

This approach requires developing new mathematical foundations to rigorously handle:

Total ordering on non-scalar objects

Distance/metric properties without explicit coordinate systems

Decidability proofs for the comparison framework

Integration with existing problem domains currently formulated in scalar arithmetic

If we can solve the problem of mapping $A$ and $B$ to a space where the comparison and the resulting "total order" are always less computationally expensive than scalar decomposition (even in the most chaotic cases), then we truly have a new mathematical foundation in our hands.


Expected Outcome :

A foundational mathematical system enabling expression-native computation at speed and decidability to exceeding scalar-based approaches, while preserving structural information lost in traditional decomposition.


**Giải thích kỹ thêm bằng Tiếng Việt :**

Đây là cổ điển :



Expressions → Computation → Scalar values



Thì ta biết được rằng lý do duy nhất để cần Scalars là :



1. "distance" or "gap" between scalars (Hẳn là liên quan chặt với Total Order & Trục tọa độ số thực chẳng hạn)



2. Any two scalars must be comparable using {<, >, =}



Vậy thì tại sao không tạo ra một không gian toán học thực sự cực kỳ mới, chưa từng ghi nhận và nó có thể :



Không cần tính ra scalars, có thể sử dụng trực tiếp Expressions và nó có thể so sánh {<,>,=} và cả "distance" or "gap" between expressions & "Total Order" (hãy để ý dấu ngoặc kép của tôi, vì nó chỉ là gần giống vậy thôi, tuy nhiên nó cực kỳ mạnh và cách mạng, nhớ điều đó) ;



Và tốc độ là khủng khiếp, vì nó vứt luôn bước "Computation" (nếu so sánh với xử lý cổ điển) ; Đơn giản là vì dùng thẳng Expressions ;


Hệ thống này có thể chạy trên kiến trúc phần cứng nhị phân (0-1) cổ điển thông qua một lớp phần mềm/trình biên dịch hoàn toàn mới chăng ? ;

Lưu ý rằng chúng ta sẽ phải đối mặt với việc tạo ra một không gian toán học mà ở đó bản thân các Biểu thức (Expressions) mang sẵn thuộc tính hình học/topo để lộ ra 3 điều trên (Comparability, "Total Order", "Distance"), thì quá trình tính toán cơ học (Computation) bị loại bỏ hoàn toàn.


**Some clues are provided, however, please note that these are only "clues" and not the solution:**


Câu hỏi : "Nếu chúng ta tạm gác lại các con số truyền thống, hình dung ra được một mô hình hoặc "hình dáng" không gian nào có thể biểu diễn được một phép nhân so với một phép cộng, để khi nhìn vào cấu trúc của chúng, ta lập tức thấy được khoảng cách (gap) mà không cần phải làm toán trông như nào ?"

Trả lời :

Dùng thẳng hệ unary (nhất phân) ; Tức là kiểu như :

Nhìn nhé :

Biểu thức A :

1 + 2 = B

Biểu thức B :

2 + 2 = B

Không gian toán học cấu trúc hình học :

A -> 111

B -> 1111

Ngay lập tức thấy được những gì ta cần thấy ; Tuy nhiên nó mới chỉ là một phần cực kỳ nhỏ của khung lý thuyết chúng ta đang cần tìm thôi ; 

Hệ nhất phân (Unary) có lẽ là ví dụ nguyên thủy nhất của việc biến "Giá trị" (Value) thành "Độ đo vật lý/Hình học" (Physical Length/Metric).

Trong không gian Unary 1 chiều này, tính toán cơ học (Computation) thực sự bị triệt tiêu, nhường chỗ cho sự đối chiếu hình dáng.

Tuy nhiên, như tôi đã tự nhận định, đây mới chỉ là một góc siêu nhỏ của khung lý thuyết. Tại sao hệ Unary không thể là câu trả lời cuối cùng ? :

Đó là vì nó gặp khó khăn với một định đề cốt lõi trong bản sketch: "Computational cost: far superior to scalar computation" (Chi phí tính toán phải vượt trội hơn tính toán vô hướng). Và vấn đề "Bùng nổ không gian biểu diễn" ;

Hãy thử đưa hệ Unary vào một "bài kiểm tra thực tế" (Stress test):

Biểu thức $C = 1000 \times 1000$

Biểu thức $D = 10^6 + 1$

Nếu dùng hệ Unary thuần túy để xây dựng không gian này, máy tính sẽ phải sinh ra một chuỗi gồm 1 triệu chữ số 1 cho biểu thức C. Quá trình bạn sinh ra các chữ số 1 đó, hay nói cách khác là "giải nén" (unroll) biểu thức thành chuỗi Unary, thực chất lại chính là Computation. Mặc dù chúng ta có thể tận dụng Kỹ thuật (cụ thể là tính toán song song), tuy nhiên nó không hề ổn.

Hệ vô hướng (Nhị phân - Binary/Scalar) chỉ cần khoảng 20 bit (chưa tới 3 byte) để biểu diễn số 1 triệu, và mất đúng 1 chu kỳ xung nhịp của CPU để so sánh. Trong khi đó, hệ Unary tốn $O(V)$ không gian bộ nhớ (với $V$ là giá trị của biểu thức) – một sự bùng nổ dữ liệu không thể kiểm soát.

Nếu như câu hỏi là : "Làm sao để có thể tránh được việc bùng nổ bộ nhớ của unary?"

Thì có một cách cực kỳ tối ưu đó là sử dụng scalar, bạn hiểu ý tôi mà, đếm "số lượng số '1'" và biến nó thành scalar thôi ;

Cơ mà nếu làm việc đó thì lại thành vô nghĩa.

Thực tế ý nghĩa của 2 câu hỏi và 2 câu trả lời trên là để chứng minh rằng 2 câu hỏi độc lập đều có 2 câu trả lời độc lập khả thi. Và chúng ta còn phải tìm nhiều điểm khác nữa, và giao thoa chúng, tạo ra một nền tảng toán học thật sự mới để thống nhất và đạt được mục tiêu ?

