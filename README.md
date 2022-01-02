# 8255-interface
With a 8086 µP , it is desired to drive a 7-segment display and 4x3 key scanning circuit by placing 8255 PPI on consecutive even addresses starting from 0A8H address.
The circuit to be implemented is a simple lock case circuit and works as follows:
1) When the lock case is unlocked, 7seg should display "U".
2) If the lock case is unlocked, it is locked by pressing the square key after entering the 4-digit password by the user.
3) When the lock case is locked, 7seg should display "L".
4) The locked case can only be opened with the password used during the lock phase or with a specific 4-digit master unlock-key. As soon as one of these two 4-digit pins are entered, the lock case opens without the need to press any other key.
5) After the lock case is opened, the system returns to the beginning and can be locked with another 4 pins.
6) If more than 4 keys are pressed during locking, the system will be reset.

Bonus point: Adding a brute-force protection to the system. (the lock case can only be opened with the master-unlock-key after 5 wrong attempts)
