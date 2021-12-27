# generic-production-transportation-IP
A simple Production and Transportation Problem solved in Lingo 19.0.

Problem Description: This is a generic problem that comes accross in Integer Programming courses. Given a problem description and the associated data, a model and a solution should be derived. A company called "ABC S.A." produces 3 products in 3 factories and supplys them to 3 different markets. Given the indices k = 1, 2, 3, i = 1, 2, 3 and j = 1, 2, 3, derive an Integer Programming problem and derive a solution using Lingo software so that the overall production and transportation costs are minimized. Please consider the following data tables: 

Cost of production for a single unit of product `k` at factory `i`:
|   | k = 1 | k = 2 | k = 3 |
--- | --- | --- | --- |
i = 1 | 3 | 5 | 5 |
i = 2 | 5 | 4 | 2 |
i = 3 | 4 | 6 | 5 |

Cost of transportation of product `k` from factory `i` to market `j = 1`:
|   | k = 1 | k = 2 | k = 3 |
--- | --- | --- | --- |
i = 1 | 2 | 4 | 6 |
i = 2 | 4 | 5 | 2 |
i = 3 | 5 | 3 | 4 |

Cost of transportation of product `k` from factory `i` to market `j = 2`:
|   | k = 1 | k = 2 | k = 3 |
--- | --- | --- | --- |
i = 1 | 5 | 3 | 3 |
i = 2 | 2 | 2 | 5 |
i = 3 | 4 | 6 | 4 |

Cost of transportation of product `k` from factory `i` to market `j = 3`:
|   | k = 1 | k = 2 | k = 3 |
--- | --- | --- | --- |
i = 1 | 2 | 5 | 4 |
i = 2 | 3 | 5 | 2 |
i = 3 | 6 | 4 | 3 |

Set-up cost for production of product `k` at factory `i`:
|   | k = 1 | k = 2 | k = 3 |
--- | --- | --- | --- |
i = 1 | 20 | 35 | 50 |
i = 2 | 30 | 40 | 25 |
i = 3 | 40 | 45 | 35 |

Maximum output production for product `k` at factory `i`:
|   | k = 1 | k = 2 | k = 3 |
--- | --- | --- | --- |
i = 1 | 500 | 950 | 900 |
i = 2 | 400 | 900 | 850 |
i = 3 | 900 | 850 | 950 |

Minimum output production for product `k` at factory `i` (in the case that we have non-zero production):
|   | k = 1 | k = 2 | k = 3 |
--- | --- | --- | --- |
i = 1 | 10 | 5 | 8 |
i = 2 | 5 | 10 | 5 |
i = 3 | 4 | 5 | 4 |

Capacity required (in man-hours) for the production of product `k` at factory `i`:
|   | k = 1 | k = 2 | k = 3 |
--- | --- | --- | --- |
i = 1 | 2 | 2 | 3 |
i = 2 | 3 | 1 | 2 |
i = 3 | 4 | 2 | 3 |

Total capacity (in man-hours) for factory `i`:
| i = 1 | i = 2 | i = 3 |
| --- | --- | --- |
| 2000 | 3500 | 5000 |

Demand for product `k` in market `j`:
|   | k = 1 | k = 2 | k = 3 |
--- | --- | --- | --- |
j = 1 | 200 | 350 | 500 |
j = 2 | 300 | 400 | 250 |
j = 3 | 400 | 450 | 350 |

Additionally, the next two constraints should be considered:
a) Any single factory can not produce more than 2 products.
b) Any single product can not be produced in more than 2 factories.

```math
<img src="https://render.githubusercontent.com/render/math?math=e^{i \pi} = -1">
```
