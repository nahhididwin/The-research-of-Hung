
(vietnamese)

**Authors:** Hung Dinh Phu Dang  

**Date:** 17-18, June 2026  

Ý tôi muốn nói là phải giải quyết được bài toán bên dưới một cách cực kỳ "thanh lịch" thông qua việc tạo ra một nền tảng không gian toán học mới :

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


Giải thích kỹ thêm bằng Tiếng Việt :

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
