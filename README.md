Download Link: https://assignmentchef.com/product/solved-ecen5013-homework-5
<br>
For this homework, both Canvas and Github online materials need to be submitted. ​<strong>Turn in a *.pdf for your report to this assignment to Canvas. Please neatly format submissions with your name, date, homework # and a link to your git repo at the top, and enumerate your answers using headings indicating each problem number, </strong>​<strong>captions explaining images and screen captures, etc. </strong>




<h1>1         Reading &amp; Resources TBD</h1>

These are reading assignments that are good to complete the homework for the week as well as review materials.

<ul>

 <li>FreeRTOS API Reference <u>​</u><a href="https://www.freertos.org/a00106.html">https://www.freertos.org/a00106.html</a></li>

</ul>







Resources:

These sections are not required but may help with doing the homework assignments.

<ul>

 <li><a href="http://processors.wiki.ti.com/index.php/Creating_IoT_Solutions_with_the_TM4C1294XL_Connected_LaunchPad_Workshop">http://processors.wiki.ti.com/index.php/Creating_IoT_Solutions_with_the_TM4C1294XL_Conne </a><a href="http://processors.wiki.ti.com/index.php/Creating_IoT_Solutions_with_the_TM4C1294XL_Connected_LaunchPad_Workshop">cted_LaunchPad_Workshop</a></li>

 <li><a href="http://software-dl.ti.com/trainingTTO/trainingTTO_public_sw/Tiva_CLP/CLP_Workbook.pdf">http://software-dl.ti.com/trainingTTO/trainingTTO_public_sw/Tiva_CLP/CLP_Workbook.pdf</a></li>

 <li>Link to download required software ​<a href="https://www.ti.com/tool/SW-TM4C">http://www.ti.com/tool/SW-TM4C</a></li>

</ul>







<h1>2         Problem Set</h1>

<strong>[Problem 1 – 30 Pts] Task creation and I2C on TI TIVA </strong>

For this problem you need to get FreeRTOS working on the TI TIVA board and be able to read temperature values from the TMP102 sensor used in project 1.




The requirements are

<ul>

 <li>Create three tasks in FreeRTOS – Temperature Task, LED Task, Logger Task</li>

 <li>The temperature task should read temperature values from the TMP102 sensor at a frequency of 1Hz.</li>

 <li>The temperature value read along with a timestamp should be passed as a structure to the logger task using FreeRTOS IPC mechanism.</li>

 <li>The LED Task should toggle LEDs D1 and D2 on the TIVA board at a frequency of 10Hz, and pass a structure containing a time stamp, toggle count and your name to the Logger task using a FreeRTOS mechanism.</li>

 <li>The logger task should receive the messages from both the above tasks and log these values to UART so that the logs can be viewed on the HOST machine.</li>

 <li>You can use either TIVA hardware timers or FreeRTOS soft timers to get the required timing for the tasks and timestamps.</li>

 <li>The timestamps should have millisecond resolution.</li>

</ul>




<strong>BONUS:</strong> Create an alert task which would be notified only when temperature goes above some​  threshold (preferably using some FreeRTOS API). This task must log some kind of alert statements to UART until temperature is out of the normal range. (3 points)










<strong>Include in your report: </strong>

<ul>

 <li><strong>A link to your project’s git repo. </strong></li>

 <li><strong>A scope shot of the LED pin switching at the required frequency. </strong></li>

 <li><strong>Screenshots of UART terminal on HOST machine showing log output of both tasks 4) (BONUS) If attempting, Screenshot of UART terminal showing alert. </strong></li>

</ul>