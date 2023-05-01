# Comparing `tmp/Pydule-3.2.8.tar.gz` & `tmp/Pydule-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pydule-3.2.8.tar", last modified: Thu Apr 27 14:59:31 2023, max compression
+gzip compressed data, was "Pydule-3.2.9.tar", last modified: Mon May  1 07:45:24 2023, max compression
```

## Comparing `Pydule-3.2.8.tar` & `Pydule-3.2.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 14:59:31.304947 Pydule-3.2.8/
--rw-rw-rw-   0        0        0     2372 2023-04-27 14:59:31.289327 Pydule-3.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1584 2023-04-27 14:15:29.000000 Pydule-3.2.8/README.md
--rw-rw-rw-   0        0        0       42 2023-04-27 14:59:31.304947 Pydule-3.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1306 2023-04-27 14:58:00.000000 Pydule-3.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 14:59:31.195598 Pydule-3.2.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 14:59:31.289327 Pydule-3.2.8/src/Pydule.egg-info/
--rw-rw-rw-   0        0        0     2372 2023-04-27 14:59:30.000000 Pydule-3.2.8/src/Pydule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-04-27 14:59:30.000000 Pydule-3.2.8/src/Pydule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 14:59:30.000000 Pydule-3.2.8/src/Pydule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2023-04-27 14:59:30.000000 Pydule-3.2.8/src/Pydule.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 14:59:30.000000 Pydule-3.2.8/src/Pydule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9767 2023-04-27 14:56:24.000000 Pydule-3.2.8/src/Pydule.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:45:24.964952 Pydule-3.2.9/
+-rw-rw-rw-   0        0        0     2419 2023-05-01 07:45:24.949329 Pydule-3.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1631 2023-04-30 15:24:02.000000 Pydule-3.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 07:45:24.964952 Pydule-3.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1399 2023-04-30 15:23:25.000000 Pydule-3.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:45:24.839980 Pydule-3.2.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 07:45:24.949329 Pydule-3.2.9/src/Pydule.egg-info/
+-rw-rw-rw-   0        0        0     2419 2023-05-01 07:45:24.000000 Pydule-3.2.9/src/Pydule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-05-01 07:45:24.000000 Pydule-3.2.9/src/Pydule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 07:45:24.000000 Pydule-3.2.9/src/Pydule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-05-01 07:45:24.000000 Pydule-3.2.9/src/Pydule.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-01 07:45:24.000000 Pydule-3.2.9/src/Pydule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12126 2023-05-01 04:34:10.000000 Pydule-3.2.9/src/Pydule.py
```

### Comparing `Pydule-3.2.8/PKG-INFO` & `Pydule-3.2.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pydule
-Version: 3.2.8
+Version: 3.2.9
 Summary: Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..
 Author: D.Tamil Mutharasan
 Keywords: python,PyDule,Module,Pydule,pydule,matrix,qrcode,youtube,weather,list,tuple,set,dictionary,clear,color,pick_color,open,app,search,play,mp3,song,restart,system,shutdown,date,time,text_to_speech,text,speech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -17,14 +17,15 @@
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)                 
 [![Python 3.6](https://img.shields.io/badge/python-3.10.7-blue.svg)](https://www.python.org/downloads/release/python-3107/)   
 
 ## Functionality of Pydule
 
 - Download Mp3 or Mp4 From Youtube
 - Encode and Decode a String
+- Record Screen,Internal Audio and Microphone
 - Seperate String
 - Swap Dictionary's Key to Values and Values to Key
 - Insert Elements in Tuple & String
 - Generate Qrcode
 - Copy Text
 - Text Translation
 - Edit JSON Files
```

### Comparing `Pydule-3.2.8/README.md` & `Pydule-3.2.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)                 
 [![Python 3.6](https://img.shields.io/badge/python-3.10.7-blue.svg)](https://www.python.org/downloads/release/python-3107/)   
 
 ## Functionality of Pydule
 
 - Download Mp3 or Mp4 From Youtube
 - Encode and Decode a String
+- Record Screen,Internal Audio and Microphone
 - Seperate String
 - Swap Dictionary's Key to Values and Values to Key
 - Insert Elements in Tuple & String
 - Generate Qrcode
 - Copy Text
 - Text Translation
 - Edit JSON Files
```

### Comparing `Pydule-3.2.8/setup.py` & `Pydule-3.2.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open('README.md','r') as fh:
 	long_description = fh.read()
 
 setup(
 	name='Pydule',
-	version='3.2.8',
+	version='3.2.9',
 	description="Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..",
 	author='D.Tamil Mutharasan',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	packages=setuptools.find_packages(),
 	keywords=['python','PyDule','Module','Pydule','pydule','matrix','qrcode','youtube','weather','list','tuple','set','dictionary','clear','color','pick_color','open','app','search','play','mp3','song','restart','system','shutdown','date','time','text_to_speech','text','speech'],
 	classifiers=[
@@ -31,11 +31,17 @@
 		'datetime',
 		'requests',
 		'AppOpener',
 		'deep_translator',
 		'qrcode',
 		'pytube',
 		'numpy',
-		'pyperclip'
+		'pyperclip',
+		'soundfile',
+		'soundcard',
+		'pyautogui',
+		'pyaudio',
+		'wave',
+		'opencv-python'
 	]
 
 )
```

### Comparing `Pydule-3.2.8/src/Pydule.egg-info/PKG-INFO` & `Pydule-3.2.9/src/Pydule.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pydule
-Version: 3.2.8
+Version: 3.2.9
 Summary: Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..
 Author: D.Tamil Mutharasan
 Keywords: python,PyDule,Module,Pydule,pydule,matrix,qrcode,youtube,weather,list,tuple,set,dictionary,clear,color,pick_color,open,app,search,play,mp3,song,restart,system,shutdown,date,time,text_to_speech,text,speech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -17,14 +17,15 @@
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)                 
 [![Python 3.6](https://img.shields.io/badge/python-3.10.7-blue.svg)](https://www.python.org/downloads/release/python-3107/)   
 
 ## Functionality of Pydule
 
 - Download Mp3 or Mp4 From Youtube
 - Encode and Decode a String
+- Record Screen,Internal Audio and Microphone
 - Seperate String
 - Swap Dictionary's Key to Values and Values to Key
 - Insert Elements in Tuple & String
 - Generate Qrcode
 - Copy Text
 - Text Translation
 - Edit JSON Files
```

### Comparing `Pydule-3.2.8/src/Pydule.py` & `Pydule-3.2.9/src/Pydule.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,92 @@
 
 err='\n \U0000274C Something Went Wrong \U0000274C\n'
 
 def openapp(appname):
 	from AppOpener import open
 	open(appname)
 
+def recintaudio(sec):
+	if isinstance(sec,int):
+		if sec>0:
+			import soundcard as sc
+			import soundfile as sf
+			import datetime
+
+			out = "Pydule Recorded Internel Audio-" + str(datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S")) + ".wav"
+			rate=48000
+
+			with sc.get_microphone(id=str(sc.default_speaker().name),include_loopback=True).recorder(samplerate=rate) as mic:
+				data=mic.record(numframes=rate*sec)
+				sf.write(file=out,data=data[:,0],samplerate=rate)
+		else:
+			print(err)
+	else:
+		print(err)		
+
+def recscreen():
+	import pyautogui
+	import cv2
+	import numpy as np
+	import datetime
+
+	screen_size = pyautogui.size()
+
+	filename = "Pydule Recorded Screen-" + str(datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S")) + ".avi"
+	fourcc = cv2.VideoWriter_fourcc(*"XVID")
+
+	out = cv2.VideoWriter(filename, fourcc, 20.0, screen_size)
+
+	cv2.namedWindow("Recording", cv2.WINDOW_NORMAL)
+
+	cv2.resizeWindow("Recording", 480, 270)
+
+	while True:
+		img = pyautogui.screenshot()
+
+		frame = np.array(img)
+
+		frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
+
+		out.write(frame)
+
+		cv2.imshow('Live', frame)
+
+		if cv2.waitKey(1) == ord('q'):
+			break
+
+	out.release()
+	cv2.destroyAllWindows()
+
+def recmic(sec):
+	import pyaudio
+	import wave
+	audio=pyaudio.PyAudio()
+	stream=audio.open(format=pyaudio.paInt16,channels=1,rate=44100,input=True,frames_per_buffer=1024)
+	frames=[]
+	fn = "Pydule Recorded Microphone-" + str(datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S")) + ".wav"
+	for i in range(0,int(44100/1024*(sec+1))):
+		data=stream.read(1024)
+		frames.append(data)
+
+	stream.stop_stream()
+	stream.close()
+	audio.terminate()
+
+	sound_file=wave.open(fn,'wb')
+	sound_file.setnchannels(1)
+	sound_file.setsampwidth(audio.get_sample_size(pyaudio.paInt16))
+	sound_file.setframerate(44100) 
+	sound_file.writeframes(b''.join(frames))
+	sound_file.close()   
+
+def mulmatrix(x,y):
+	import numpy as np
+	return np.dot(np.array(x), np.array(y))
+
 def swapdict(d):
 	if isinstance(d,dict):
 		new={}
 		for i in d:
 			new[d.get(i)]=i
 		return new
 
@@ -27,46 +105,52 @@
 	for i in st:
 		if len(s)!=n:
 			s+=i
 		else:
 			l+=[s]
 			s=''
 			s+=i
-	if len(s)>=0:
+	if len(s)>0:
 		l+=[s]          
 	return l 
 
-def dcodestr(st,key):
-	s=''
+def dcodestr(st,k):
+	s,key='',{}
 	if isinstance(st,str):
+		for j in k:
+			n=chr(k[j])
+			key[j]=n
 		sr=sepstr(st,7)
 		for i in range(len(sr)):
 			s+=key[sr[i]]
 		return s
 	else:
 		print(err)    
 
 def codestr(string):
 	import random as r
 	ex=['!','@','#','$','%','^','&','*','_','=','-','+']
-	s,Ans,d='',[],{'A': None, 'B': None, 'C': None, 'D': None, 'E': None, 'F': None, 'G': None, 'H': None, 'I': None, 'J': None, 'K': None, 'L': None, 'M': None, 'N': None, 'O': None, 'P': None, 'Q': None, 'R': None, 'S': None, 'T': None, 'U': None, 'V': None, 'W': None, 'X': None, 'Y': None, 'Z': None, 'a': None, 'b': None, 'c': None, 'd': None, 'e': None, 'f': None, 'g': None, 'h': None, 'i': None, 'j': None, 'k': None, 'l': None, 'm': None, 'n': None, 'o': None, 'p': None, 'q': None, 'r': None, 's': None, 't': None, 'u': None, 'v': None, 'w': None, 'x': None, 'y': None, 'z': None,'1':None,'2':None,'3':None,'4':None,'5':None,'6':None,'7':None,'8':None,'9':None,'0':None,'!':None,'@':None,'#':None,'$':None,'%':None,'^':None,'&':None,'*':None,'_':None,'=':None,'-':None,'+':None,'(':None,')':None,'[':None,']':None,'`':None,'~':None,'{':None,'}':None,'?':None,'\\':None,'\'':None,'/':None,';':None,':':None,'\"':None,'<':None,'>':None,'.':None,',':None,' ':None}
+	s,Ans,d,e='',[],{'A': None, 'B': None, 'C': None, 'D': None, 'E': None, 'F': None, 'G': None, 'H': None, 'I': None, 'J': None, 'K': None, 'L': None, 'M': None, 'N': None, 'O': None, 'P': None, 'Q': None, 'R': None, 'S': None, 'T': None, 'U': None, 'V': None, 'W': None, 'X': None, 'Y': None, 'Z': None, 'a': None, 'b': None, 'c': None, 'd': None, 'e': None, 'f': None, 'g': None, 'h': None, 'i': None, 'j': None, 'k': None, 'l': None, 'm': None, 'n': None, 'o': None, 'p': None, 'q': None, 'r': None, 's': None, 't': None, 'u': None, 'v': None, 'w': None, 'x': None, 'y': None, 'z': None,'1':None,'2':None,'3':None,'4':None,'5':None,'6':None,'7':None,'8':None,'9':None,'0':None,'!':None,'@':None,'#':None,'$':None,'%':None,'^':None,'&':None,'*':None,'_':None,'=':None,'-':None,'+':None,'(':None,')':None,'[':None,']':None,'`':None,'~':None,'{':None,'}':None,'?':None,'\\':None,'\'':None,'/':None,';':None,':':None,'\"':None,'<':None,'>':None,'.':None,',':None,' ':None},{}
 	while True:
 		if len(Ans)!=95:
 			n=''
 			for i in range(7):
 				n+=ex[r.randint(0,11)]
 			if n not in Ans:
 				Ans+=[n]
 		else:
 			break
 	for i,j in zip(d,Ans):
 		d[i]=j                
 	for i in string:
 		s+=d[i]
-	return s,d
+	for i in d:
+		n=ord(i)
+		e[n]=d[i]	
+	return s,e
 
 def wjson(data,path):
 	import json
 	with open(path,'w') as json_file:
 		json.dump(data,json_file)
 
 def deljsonele(path):
@@ -86,23 +170,23 @@
 	v=eval(input('Enter the Value : '))
 	copy[k]=v
 	with open(path,'w') as json_file:
 		json.dump(copy,json_file)
 
 def num(n):
 	if isinstance(n,int):
-		if n==1:
-			n='1st'
-		elif n==2:
-			n='2nd'
-		elif n==3:
-			n='3rd'
+		if str(n).endswith('1') and not(str(n).endswith('11')):
+			s=str(n)+'st'
+		elif str(n).endswith('2') and not(str(n).endswith('12')):
+			s=str(n)+'nd'
+		elif str(n).endswith('3') and not(str(n).endswith('13')):
+			s=str(n)+'rd'        
 		else:
-			n=str(n)+'th'
-		return n
+			s=str(n)+'th'
+		return s 
 	else:
 		print(err)	
 def intuple(x,index,element):
 	if isinstance(x,tuple):
 		new=()
 		if len(x)<=index:
 			new+=x+(element,)
@@ -128,15 +212,15 @@
 				else:
 					new+=j
 		return new
 	else:
 		print(err)			
 
 def functions():
-	l=['codestr(<str>)','dcodestr(<str>,<dict>)','swapdict(<dict>)','sepstr(<str>)','wjson(<dict>,<path>)','deljsonele(<path>)','upjson(<path>)','copytext(<text_to_copy>)','translate(<sentence>,<language>)','ytmp4(<youtube_link>)','ytmp3(<youtube_link>)','cqrcode(<link>)','summatrix(<matrix a>,<matrix b>)','submatrix(<matrix a>,<matrix b>)','intuple(<tuple>,<index>,<new_element>)','instr(<str>,<index>,<new_element>)','reSet(<old_set>,<new_element>,<old_element>)','reStr(<old_str>,<index>,<new_str>)','reDict(<old_dict>,<old_key>,<new_key>)','reList(<old_list>,<index>,<new_element>)','reTuple(<old_tuple>,<index>,<new_element>)','clist(<length_of_the_list>)','ctuple(<length_of_the_tuple>)','cdict(<length_of_the_dict>)','cset(<length_of_the_set>)','pickcolor()','search(<content>)','playsong(<path>)','restart_system()','shutdown_system()','datetoday()','timenow()','say(<content>)','openfile(<path>)','weathernow(<city_name>)','setvoice(<number_between 0 to 2>)','voicerate(<any_number>)']
+	l=['recintaudio(<seconds>)','recmic(<seconds>)','recscreen()','mulmatrix(<matrix a>,<matrix b>)','codestr(<str>)','dcodestr(<str>,<dict>)','swapdict(<dict>)','sepstr(<str>)','wjson(<dict>,<path>)','deljsonele(<path>)','upjson(<path>)','copytext(<text_to_copy>)','translate(<sentence>,<language>)','ytmp4(<youtube_link>)','ytmp3(<youtube_link>)','cqrcode(<link>)','summatrix(<matrix a>,<matrix b>)','submatrix(<matrix a>,<matrix b>)','intuple(<tuple>,<index>,<new_element>)','instr(<str>,<index>,<new_element>)','reSet(<old_set>,<new_element>,<old_element>)','reStr(<old_str>,<index>,<new_str>)','reDict(<old_dict>,<old_key>,<new_key>)','reList(<old_list>,<index>,<new_element>)','reTuple(<old_tuple>,<index>,<new_element>)','clist(<length_of_the_list>)','ctuple(<length_of_the_tuple>)','cdict(<length_of_the_dict>)','cset(<length_of_the_set>)','pickcolor()','search(<content>)','playsong(<path>)','restart_system()','shutdown_system()','datetoday()','timenow()','say(<content>)','openfile(<path>)','weathernow(<city_name>)','setvoice(<number_between 0 to 2>)','voicerate(<any_number>)']
 	print('Available Functions : \n')
 	for i in l:
 		print(f'\t{i}')
 
 def summatrix(x,y):
 	import numpy as np
 	result = np.array(x) + np.array(y)
@@ -183,15 +267,15 @@
 	
 def cqrcode(data,filename):
 	import qrcode
 	img = qrcode.make(data)
 	img.save(filename)
 	print('\nQrcode Saved Successfully \U00002714\n')
 	
-def info():
+def Author():
 	print('\nThis Pydule is Created by D.Tamil Mutharasan \U0001F608\n')
 
 def reStr(oldstr,index,newstr):
 	if isinstance(oldstr,str):
 		new=''
 		for i in range(len(oldstr)):
 			if i==index:
@@ -257,15 +341,15 @@
 	return Tuple
 
 def cdict(mx):
 	Dict={}
 	print('Enter Values One by One \U0001F447\n')
 	for i in range(mx):
 		key=eval(input(f'Enter the Key of No.{num(i+1)} Element :'))
-		value=eval(input(f'Enter the Value of No.{num(i+1)} Element :'))
+		value=eval(input(f'Enter the Value of {key} Element :'))
 		print()
 		Dict[key]=value
 	print('Dictionary Created Successfully \U00002714')	
 	return Dict
 
 def cset(mx):
 	Set=set()
```

