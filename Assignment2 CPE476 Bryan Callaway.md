**Code to move the rover in a circle:**

`from romipi_astar.romipi_driver import AStar`
`import sys`
`import time`

`romi = AStar()`

`def circle():`

```python
    romi.twist(0,10)
```



`x=1`



**Code to move the rover in a square:**



`from romipi_astar.romipi_driver import AStarimport sysimport time``

``romi = AStar()`

`def square():`
        `romi.twist(2,0)`
        `time.sleep(2)`
        `romi.twist(0,10)`
        `time.sleep(2)`
        `romi.twist(2,0)`
        `time.sleep(2)`
        `romi.twist(0,10)`
        `time.sleep(2)`



`x=1`
`while True:`
        `square()`
        `x+=1`