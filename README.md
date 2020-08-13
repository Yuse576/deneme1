#python 3.7.1
print("şifrenizi öğrenebilir miyim?")
sifre=input("şifre: ")

def notgir():
    ad=input("isim: ")
    soyad=input("soyisim: ")
    not1=input("not1: ")
    not2=input("not2: ")
    not3=input("not3: ")
    with open("ogrencinotlari.txt","a",encoding="utf-8") as dosya:
        dosya.write(ad+" "+soyad+":"+not1 +"," + not2 + ","+ not3+"\n")
def notlarioku():
    with open("ogrencinotlar.txt","r",encoding="utf-8") as dosya:
        for satir in dosya:
            print(satir)

        
        
        
        def notkayıt():
             pass
    
    
while sifre=="2801":
    islem=input("1-notları oku\n2-not gir\n3-notları kayıt et\n4-çıkış")
    if islem=="1":
        notlarioku()
    elif islem=="2":
        notgir()
    elif islem=="3":
        notkayıt()
    else:
        print("yanlış bir işlem yaptınız (HATA)")
        break



