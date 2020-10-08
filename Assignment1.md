**Code to move the robot in a circle:**

`#include <Romi32U4.h>`

`Romi32U4Motors motors;`
`Romi32U4ButtonA buttonA;`

`void setup()`
`{`
  `// Wait for the user to press button A.`
  `buttonA.waitForButton();`

  `// Delay so that the robot does not move away while the user is`
  `// still touching it.`
  `delay(1000);`
`}`

`void loop()`
`{`
 `for (int i = 0; i <= 4; i++)`
  `{`
    `motors.setLeftSpeed(200);`
    `motors.setRightSpeed(50);`
    `delay(2000);`

  `}`

`}`

**Code to move the robot in a square:**

`#include <Romi32U4.h>`

`Romi32U4Motors motors;`
`Romi32U4ButtonA buttonA;`

`void setup()`
`{`
  `// Wait for the user to press button A.`
  `buttonA.waitForButton();`

  `// Delay so that the robot does not move away while the user is`
  `// still touching it.`
  `delay(1000);`
`}`

`void loop()`
`{`
`for (int i = 0; i <= 4; i++)`
  `{`
    `motors.setLeftSpeed(200);`
    `motors.setRightSpeed(200);`
    `delay(2000);`
    `motors.setLeftSpeed(100);`
    `motors.setRightSpeed(50);`
    `delay(2000);`
    `motors.setLeftSpeed(200);`
    `motors.setRightSpeed(200);`
    `delay(1000);`
    `motors.setLeftSpeed(100);`
    `motors.setRightSpeed(50);`
    `delay(2000);`
  `}`

  `delay(500);`
`}`