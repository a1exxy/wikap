```
htpasswd -bnBC 10 "" passwordExample | tr -d ':\n'

$2y$10$65xw23DFQqEDge3yPN/3GOH4be9xXpNJ7MYJrDld7uTR/5L84QRcG
```




c пользователем:

```
htpasswd -bnBC 10 "USERNAME" passwordExample

USERNAME:$2y$10$E6IcqpocMD1YFC1aHIwwF.R5XF6rc/3bL44Tc/NoXspTkwKLfm9Cu
```