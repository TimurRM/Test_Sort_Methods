``` ini

BenchmarkDotNet=v0.13.1, OS=Windows 10.0.19044.1826 (21H2)
Intel Core i7-4790 CPU 3.60GHz (Haswell), 1 CPU, 8 logical and 4 physical cores
.NET SDK=6.0.302
  [Host]     : .NET 6.0.7 (6.0.722.32202), X64 RyuJIT  [AttachedDebugger]
  DefaultJob : .NET 6.0.7 (6.0.722.32202), X64 RyuJIT


```
|              Method |       Mean |     Error |    StdDev | Rank |  Gen 0 | Allocated |
|-------------------- |-----------:|----------:|----------:|-----:|-------:|----------:|
|       TestQuickSort |  52.057 μs | 0.4040 μs | 0.3779 μs |    3 | 0.9155 |      4 KB |
|      TestBubbleSort | 806.328 μs | 7.5836 μs | 7.0937 μs |    6 |      - |      4 KB |
|   TestSelectionSort | 361.954 μs | 6.0960 μs | 5.7022 μs |    4 | 0.4883 |      4 KB |
|    TestCountingSort |   2.798 μs | 0.0252 μs | 0.0224 μs |    1 | 0.9766 |      4 KB |
|      TestShakerSort | 686.210 μs | 6.9261 μs | 6.1398 μs |    5 |      - |      4 KB |
| TestQuickDotnetSort |   6.371 μs | 0.0596 μs | 0.0557 μs |    2 | 0.9613 |      4 KB |
