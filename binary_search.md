Overflow bug
* We often calculate mid using this formula: 
$mid=(L+R)/2$. But $L+R$ may overflow. So, we should always calculate mid using this formula:
$$mid=L+(R−L)/2$$
* Note: Here $/$ means floor division