1ci sual
def sahe(a, h):
    return 0.5 * a * h
print(sahe(3, 4))
2ci sual
def tekrarlanan_herfleri_sil(sozcuk):
    yeni_soz = ""
    for herf in sozcuk:
        if herf not in yeni_soz:
            yeni_soz += herf
    return yeni_soz

soz = "hhhhhaaaaaacccciiiii"
netice = tekrarlanan_herfleri_sil(soz)
print(netice)
3cu sual
def eded(eded):
    reqemler= set(str(eded))
    if len(reqemler) == 10:
        return "ededin icinde butun reqemler var"
    else:
        eksik_reqemler = set("0123456789") - reqemler
        return "ededlerin icinde " + str(len(eksik_reqemler)) + " rəqəm yoxdur: " + ", ".join(eksik_reqemler)

verilmis = 98305614820698024492
netice = eded(verilmis)
print(netice)
5ci sual
def bolunen(reqem):
    cem = sum(int(digit) for digit in str(reqem))
    if reqem % cem == 0:
        return f"Bəli, {reqem} ədədi {cem} ədədinə bölünür."
    else:
        return f"Xeyr, {reqem} ədədi {cem} ədədinə bölünmür."

reqem = 133
sonuc = bolunen(reqem)
print(sonuc)
7ci sual
def tam_bolunen_reqemler():
    reqemler = []
    for sayi in range(1, 100):
        if sayi % 3 == 0 and sayi % 5 == 0:
            reqemler.append(sayi)
    return reqemler

netice = tam_bolunen_reqemler()
print(netice)
8ci sual
daxil_edilmis_eded = int(input("Bir ədəd daxil edin: "))
cut_sayi = daxil_edilmis_eded // 2
print("Daxil edilmiş ədədə qədər olan cüt ədədlərin sayı:", cut_sayi)
9 cu sual
siyahi = [2, 2, 4, 3, 6, 9, 6, 1, 5, 1]

siyahi = [x for x in siyahi if x <= 3]
print(siyahi)
13 cu sual
ededler = input("Ədədləri vergül ilə ayıraraq daxil edin: ")
ededler_list = ededler.split(",")
cedvelleri = []

for eded in ededler_list:
    cedvelleri.append(int(eded))

cem = sum(cedvelleri)
print(cem)

14 cu sual
cumle = input("Cümləni daxil edin: ")
sozler = cumle.split()
son_soz = sozler[-1]
print(son_soz)
15 ci sual
reqemler = [1, 3, 4, 5, 6]
netice = []

for reqem in reqemler:
    netice.append(reqem ** 2)
print(netice)

