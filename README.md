# BonobonoTurtlebot
보노보노팀의 터틀봇 주행
영상처리 소스코드 확인
 => Turtlebot_Autorace/source/src/ImageProcess/src/

	DetectBarAndLight.cpp
	DetectParkZone.cpp
	LineTracing.cpp

## 1. Server Computer
![Alt text](/capture/1.png)
<pre><code> $ifconfig </code></pre>
![Alt text](/capture/3.png)
<pre><code> $gedit ~/.bashrc </code></pre>
![Alt text](/capture/5.png)
<pre><code> $source ~/.bashrc </code></pre>
<pre><code> $roscore </code></pre>
![Alt text](/capture/8.png)
<pre><code> $rosrun remoteControl_pkg remoteControl </code></pre>
![Alt text](/capture/10.png)


## 2. Turtlebot

Terminal-1 ( Connect Turtlebot And OpenCR ) 
<pre><code> $rosrun rosserial_python serial_node.py _port:=/dev/ttyACM0 </code></pre>

Terminal-2 ( Run LineTrace )
<pre><code> $rosrun opencv_tutorial LineTrace </code></pre>
![Alt text](/capture/lineTrace.png)

Terminal-3 ( Run BarAndLight )
<pre><code> $rosrun opencv_tutorial BarAndLight </code></pre>
![Alt text](/capture/BarAndLight.png)

Terminal-4 ( Run ParkZone )
<pre><code> $rosrun opencv_tutorial ParkZone </code></pre>
![Alt text](/capture/ParkZone.png)

## 3. OpenCR Upload 
turtlebot_openCR/turtlebot/turtlebot.ino  : File Upload
