TextWindow.WriteLine("WELCOME TO MAKBULE BANK")
TextWindow.WriteLine("Your login process starts immediatly")
TextWindow.WriteLine(". . .")
TextWindow.WriteLine("Name and surname? :")
Kullanici["isim"]=TextWindow.Read()
TextWindow.WriteLine("Whats your ID number :")
Kullanici["yaş"]=TextWindow.Read()
TextWindow.WriteLine("How much money do you deposit in your bank account? :")
D=TextWindow.Read()
TextWindow.WriteLine("Create a password for your bank account :")
C=TextWindow.ReadNumber()

TextWindow.WriteLine("YOUR INFORMATION WAS SAVED SUCCESSFULLY. HAVE A GOOD DAY.")



TextWindow.WriteLine("Welcome back to MAKBULE BANK")
TextWindow.WriteLine("Enter your password first to access your bank account.")
M=TextWindow.ReadNumber()
if M=C  then
    TextWindow.WriteLine("WELCOME")
TextWindow.WriteLine("Type what you want to do:A)UPLOAD MONEY B)WITHOUT MONEY / PLEASE NOTE CAPITAL")
islem= TextWindow.Read()
If islem="A" then 
    TextWindow.WriteLine("How much money do you want to load into your account?")
    transfer=TextWindow.ReadNumber()
    sonuca =D+transfer
TextWindow.WriteLine("Your accaunt has " + sonuca + " Dolars.")
TextWindow.WriteLine("YOUR TRANSACTION IS COMPLETED.MAKBULE BANK WISHES YOU A GOOD DAY")
ElseIf islem="B" then 
    TextWindow.WriteLine("How much money do you want to withdraw from your account?")
    cekim=TextWindow.ReadNumber()
    sonucb =D-cekim
TextWindow.WriteLine("Your accaunt has " + sonucb + " Dolars.")
TextWindow.WriteLine("YOUR TRANSACTION IS COMPLETED.MAKBULE BANK WISHES YOU A GOOD DAY")


Else
    TextWindow.WriteLine("Error restart application")

EndIf


Else
    TextWindow.WriteLine("Error restart application")
EndIf
