import random 
import string
passw=string.ascii_letters + string.digits + string.punctuation
password=list(passw)
key = password.copy()
random.shuffle(key)
kod=input("kodu daxiil et: ")   
desifr=""
for letter in kod:
    index = key.index(letter)
    desifr += password[index]

print(f"senin kodun: {kod}")

print(f"deyisdirilmis kod: {desifr}")
