# VHDL Counter Overflow Bug

This repository demonstrates a common error in VHDL code: counter overflow.  The `buggy_counter.vhd` file contains a counter that increments without checking for overflow. Once the counter reaches its maximum value (15), it continues to increment, resulting in unexpected behavior (likely wrapping around to 0).

The solution, `fixed_counter.vhd`, addresses this by adding an overflow check, ensuring that the counter stops at 15 and doesn't wrap around.