passangers = []
while True :
    passanger = input ("What is your name?:").strip()
    if passanger.upper() == "STOP":
        break
    passangers.append(passanger)
    ticket = input (f" {passanger} Do you have a ticket? : yes or no :" ).upper()
    if ticket == "NO":
        print (f"{passanger} proceed to A")
    else:
         print (f"{passanger} proceed to B")
    register= input("Should another passanger be registered? : YES or NO :").upper()
    if register == "NO":
            break


print(len(passangers))  
print (passangers)
