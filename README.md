# Typing-speed-test-
#python code real typing speed 
 #typing speed checker 
 #Create Aashish raaz kumar 
import time
String='HELLO I AM AASHISH RAAZ KUMAR I AM CREATE THIS PROGRAM CHACK YOUR TYPING SPEED'
string='CHAKE YOUR TYPING SPEED'
wordcount=len(String.split())
print(String)
while True:
    t0=time.time()
    inputtext=str(input('Enter the Sentence:'))
    t1=time.time()
    accuracy=len(set(inputtext.split())&set(String.split()))
    accuracy=accuracy/wordcount
    timetaken=t1-t0
    wpm=wordcount/timetaken
    print("WPM",wpm,"Accuracy",accuracy,"Timetaken",timetaken)
