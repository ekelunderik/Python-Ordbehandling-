# Python-Ordbehandling-

def findWord(string):
#Hittar bara ordet ensamt och är case sensitive

    Wordlist = []
    Words = []

    q = 0
    k = string
    a = open("Extentor","r")
    for line in a:
        for word in line.split():
            Wordlist.append(word)
    
    for i in range(len(Wordlist)):
        if string.lower() in Wordlist[i].lower():
            q += 1

    print(q)   
