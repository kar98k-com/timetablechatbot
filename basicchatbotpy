k=int(input("Hi friend how can i help you in following ways \n 1) making  time table \n 2)to know details of today timetable\n please enter 1 or 2\n" ))
if (k<0) or (k>2) :                           #if input is other than 1 or 2 it will rise exception
    raise Exception("Sorry you have given unknown input")
if k==1 :                               
 f=open('s1','w')           #it will create file and store in a computer  what we have given as input
 m=int(input("Hi! friend i will help in you timetable making ,please enter how many subjects you need to study  "))
 for i in range(1,m+1) :                              #it will data from user -- subject name ,time of subject need to be read
    a=input("please enter the subject name  ")
    b= input("please set  the time  you neeed to study, in the enterd way - hours : minutes AM/PM for ex: 2-23PM--3-30PPM     ")
    c=a+':'+b+"\n"
    f.write(c)            # store in a computer as text file what we have given as write() funtion
else :
   m=open('s1','r')      #it will open the stored data
   data=m.read()
   data=[k for k in data.split('\n') if len(k)>1]
   data={k.split(':')[0].strip():k.split(':')[1].strip() for k in data}  #it will seperate the string data to dictonary form
   if data.items() :
     print("Today you timetable is :-\nsubjects  ")
     for k in data.keys() :         #it will extract keys from dictoniry and print it
         print(k)
     print("\ntime to study the respective subjects")
     for k in data.values() :       #it will extract valus from dictoniry and print it
         print(k)

   else :
      print("there is no present timetable") #if files is Empity them this part willexecute
 
