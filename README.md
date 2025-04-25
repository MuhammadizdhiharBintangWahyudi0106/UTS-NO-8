# UTS-NO-8
Jawab soal no 8
def hitung_kalimat(kalimat):
    vokal = "aiueoAIUEO"
    jumlah_vokal = 0
    jumlah_konsonan = 0

    for huruf in kalimat:
        if huruf.isalpha():
            if huruf in vokal:
                jumlah_vokal += 1
            else:
                jumlah_konsonan += 1

    jumlah_kata = len(kalimat.split())

    print("Vokal   :", jumlah_vokal)
    print("Konsonan:", jumlah_konsonan)
    print("Kata    :", jumlah_kata)

kalimat = input("Masukkan kalimat: ")
hitung_kalimat(kalimat)
