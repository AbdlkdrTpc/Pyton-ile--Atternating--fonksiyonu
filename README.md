# Pyton-ile--Atternating--fonksiyonu
3 farklı yöntem ile Bir stringin indexlerinin çift veya tek sayı olmasına bağlı olarak ilgili indexteki değeri büyük harfe veya küçük harfe çeviren bir fonksiyon


# Python process
    def alternating(string):
        new_string = ""
        for string_index in range(len(string)):
            if string_index %2 == 0:
                new_string += string[string_index].upper()
            else:
                new_string += string[string_index].lower()
        print(new_string)
    alternating("bu benim ilk kod çalışmam")
    
    string = "bu benim ilk kod çalışmam"


# List comprehensions process
    x = [string[string_index].upper() if string_index %2 == 0 else string[string_index].lower() for string_index in range(len(string))]
    liste = ""
    for i in x:
        liste += i
    print(liste)


# enumerate function
    def alternative(string):
        liste = ""
        for i, v in enumerate(string):
            if i %2 == 0:
                liste += v.upper()
            else:
                liste += v.lower()
        print(liste)
    alternative("bu benim il kod çalışmam")

