import requests,random
# Dev : @Reback_Dev
# Chanel : @Hackeronion
F = '\033[2;32m' #اخضر
Z = '\033[1;31m' #احمر
X = '\033[1;33m' #اصفر
F = '\033[2;32m' #اخضر
A = '\033[2;34m'#ازرق
C = '\033[2;35m' #وردي
B = '\033[2;36m'#سمائي
Y = '\033[1;34m' #اصفر
id = input(B+'Enter Your Id => ')
tok = input(B+'Enter Your Token => ')
print(Z+'='*58)
while True :
 xx = 'qwertyuiopasdfghjklmnbvcxz'
 x2 = 'q1w2e3r4t5y6u7i8o9p0asdfghjklmnbvcxz'
 R1F= str(''.join((random.choice(xx) for i in range(2))))
 R2F= str(''.join((random.choice(x2) for i in range(2))))
 url=f"https://t.me/{R1F}_{R2F}"
 req = requests.get(url).text

 if '"tgme_username_link"' in req:
  print(f'{F}AvaLb  | {X}{R1F}_{R2F}')
  tlg = (f'''https://api.telegram.org/bot{tok}/sendMessage?chat_id={id}&text=@{R1F}_{R2F} + \n''')
  i = requests.post(tlg)    
 else:
  print(f'{Z}EROoR  | {X}{R1F}_{R2F}')
# Dev : @Reback_Dev
# Chanel : @Hackeronion
  
حسابات
