# FLOWCHART Ongkos Kirim

```mermaid
flowchart TD
Start((Start))
Input[\Jarak\]
Decision{Jarak >= 5}
ProcessLebih(TotalLebih = (Jarak - 5) * 3rb + 5rb)
ProcessKurang(TotalKurang = 5rb)
TerminatorLebih([TotalLebih])
TerminatorKurang([TotalKurang])
Stop((Stop))

Start --> Input
Input --> Decision
Decision -- YES --> ProcessLebih
Decision -- No --> ProcessKurang
ProcessLebih --> TerminatorLebih
ProcessKurang --> TerminatorKurang
TerminatorLebih & TerminatorKurang --> Stop

```
