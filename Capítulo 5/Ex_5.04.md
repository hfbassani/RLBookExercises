---
output: pdf_document
---

Lembrando que foi estabelecido que:

$Q_{n+1} = \frac{1}{n}\sum_{i=1}^{n}R_{i}$  
$Q_{n+1} = \frac{1}{n}(R_{n} + \sum_{i=1}^{n-1}R_{i})$  
$Q_{n+1} = \frac{1}{n}(R_{n} + (n-1)\frac{1}{(n-1)}\sum_{i=1}^{n-1}R_{i})$  
$Q_{n+1} = \frac{1}{n}(R_{n} + (n-1)Q_{n})$  
$Q_{n+1} = \frac{1}{n}(R_{n} + nQ_{n} - Q_{n})$  
$Q_{n+1} = Q_{n} + \frac{1}{n}(R_{n} - Q_{n})$  

De maneira similar, faremos então a modificação no algoritmo de Monte Carlo ES:

$Q_{n}(S_{t},A_{t}) = \frac{1}{n}\sum_{i=1}^{n}G_{i}(S_{t},A_{t})$  
$Q_{n}(S_{t},A_{t}) = \frac{1}{n}(G_{n}(S_{t},A_{t}) + \sum_{i=1}^{n-1}G_{i}(S_{t},A_{t}))$  
$Q_{n}(S_{t},A_{t}) = \frac{1}{n}(G_{n}(S_{t},A_{t}) + (n-1)\frac{1}{(n-1)}\sum_{i=1}^{n-1}G_{i}(S_{t},A_{t}))$  
$Q_{n}(S_{t},A_{t}) = \frac{1}{n}(G_{n}(S_{t},A_{t}) + (n-1)Q_{n-1}(S_{t},A_{t}))$   
$Q_{n}(S_{t},A_{t}) = \frac{1}{n}(G_{n}(S_{t},A_{t}) + nQ_{n-1}(S_{t},A_{t}) - Q_{n-1}(S_{t},A_{t}))$   
$Q_{n}(S_{t},A_{t}) =  Q_{n-1}(S_{t},A_{t}) + \frac{1}{n}(G_{n}(S_{t},A_{t}) - Q_{n-1}(S_{t},A_{t}))$   
