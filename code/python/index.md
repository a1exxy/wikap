import sys  for line in sys.stdin:     print line

if len(sys.argv)>1:     print('option1')

import sys data = sys.stdin.readlines()print "Counted", len(data), "lines."

import sys f = open(sys.argv[1]) if len(sys.argv) > 1 else sys.stdin     for line in f:

import os import re #a = str(os.listdir(path=".")) #print(str(os.system('grep 1qa ttt')))  f = open('ttt') p = re.compile('1qa') for line in f:     if p.match(line):         print(line,end='')

pip install impyla

#!/usr/bin/env python    from impala.dbapi import connect conn = connect(host='10.146.128.130', port=21050) cur = conn.cursor()  cur.execute('SHOW TABLES') for row in cur: 	print row[0]  print  cur.execute('describe 10_149_0_2') for row in cur: 	print row[0],"\t\t",row[1]  print print "======================================"