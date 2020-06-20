# STM32_MS5611
 STM32 driver for air pressure sensor MS5611
 
## Usage:

First, replace the delay(ms) function in ms5611.c with equivlent one.

Then,
```
#include "ms5611.h"

...

ms5611_set_i2c(&hi2c1);

...

ms5611_init();

...

while (1){
   
   ms5611_update();
   
   double temp = ms5611_get_temperature();
   double pressure = ms5611_get_pressure();
   
}

```

 I hope this will be helpful to your project!
