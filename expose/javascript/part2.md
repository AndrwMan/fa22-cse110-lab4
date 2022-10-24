13. 
A. '32'. Number 2 maps to string representation so '3' + '2' concatenates to '32'
B. 1. '3' converted to Number 3. 3 - 2 = 1.
C. 3. null converted to Number 0. 3 + 0 = 3
D. '3null'. null converted to String 'null', so '3' + 'null' concatenates to '3null'
E. 4. true converted to Number 1. 1 + 3 = 4
F. 0. Both are converted to Number 0, 0+0=0
G. '3undefined'. undefined converted to String 'undefined', so '3' + 'undefined' concatenates to '3undefined'
H. NaN. undefined converted to Number NaN, so '3' - NaN = NaN 
14. 
A. true. '2' converts to Number 2, so 2 > 1
B. false. alphabetically 2 > 1 in '2' < '(1)2'
C. true. Not checking types, 2 == 2
D. false. Checking types Number 2 !== String '2'
E. false. true as Number is 1, 1 != 2
F. true. Boolean(x) where x is positive Number will return true, true === true
15. `===` checks types javscript type matches in addition to value matching/equality (`==` only checks value).
