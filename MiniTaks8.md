# FLOWCHART Ongkos Kirim

```mermaid
flowchart TD
Start((Start))
Input[\Jarak\]
Decision{Jarak >= 5}
Lebih(Lebih = Jarak - 5)
ProcessLebih(Total = Lebih * 3000 + 8000)
ProcessKurang(Total = 8000)
Total[\Total\]
Stop(((Stop)))

Start --> Input
Input --> Decision
Decision -- Yes --> Lebih
Decision -- No --> ProcessKurang
Lebih --> ProcessLebih
ProcessKurang & ProcessLebih  --> Total
Total --> Stop
```
