---
title: Loggernet interface
---
## Connect to the Droughtbox

+ Open LoggerNet v4.1

+ __Initial connect:__ Go to Main -->  and click on Connect

	 ![Initial connect](media/loggernet_initial_connect.jpg)

+ __Connect to the Droughtbox:__ Select the Droughtbox and press Connect  

	![Connect to Droughtbox](media/loggernet_connect.jpg)

## Create a data file

+ __Create data file__:  Go back to the main interface and press the setup bottom  
 
![page_setup](media/loggernet_setup_datafile.jpg)


+ __Create a new file__: Select Droughtbox at COM32  --> Go to the Data Files tab --> Select droughtbox --> change the name of the file following the format `YYYY_MM_DATE_OWNER.dat` for example `2023_08_10_erick.dat`

+ Make sure that the `File Output Option` is set up as `Create unique file name`  

+ To save the data into the file press the `Collect Now` bottom. __This step must be done each time you want to save data__ 

+ If you don't change the file path, your data file will be stored at `C:\Campbellsci\LoggerNet` 
 
+ In case that Network Map (located at the left hand of the image below) is not as shown in the picture, click on the `View` bottom and select `Standard` to change it.


	![Create a new datafile](media/loggernet_create_data_file.jpg)


## Open the numeric display

 + __Open Num Display__: Press Num Display bottom
 
![open_numeric_display](media/loggernet_open_numerical_display.jpg)


+ This window should appear 

![numeric_display_window](media/loggernet_numeric_display.jpg)

+ The main inputs that can be change are:
	+ `SetPointT`
	+ `SetPointVPD`
	+ `SetPointAbsH`
	+ `SetPointRH`


### List of abbreviations in the numerical display 

<table>
  <tr>
   <td><strong>Term</strong>
   </td>
   <td><strong>Definition</strong>
   </td>
   <td><strong>Units</strong>
   </td>
  </tr>
  <tr>
   <td>BattV
   </td>
   <td>Voltage Battery Reading
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><em>PTempC</em>
   </td>
   <td>Logger panel temperature (room temp)
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><em>AirTC</em>
   </td>
   <td>Air temp in box measured by Temp/RH sensor (slow response)
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><em>RH</em>
   </td>
   <td>Measured relative humidity inside the box
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><em>TC</em>
   </td>
   <td>Air temp in box measured by fine wired thermocouple (fast response)
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><em>VPD</em>
   </td>
   <td>Measured vapor pressure deficit inside the box, calculated from RH and AirTc
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><em>AbsH</em>
   </td>
   <td>Measured absolute humidity inside the box, calculated from RH and AirTc 
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><em>Strain(1)</em>
   </td>
   <td>Weight measured on strain 1
   </td>
   <td>grams
   </td>
  </tr>
  <tr>
   <td><em>Strain(2)</em>
   </td>
   <td>Weight measured on strain 2
   </td>
   <td>grams
   </td>
  </tr>
  <tr>
   <td><em>Strain(3)</em>
   </td>
   <td>Weight measured on strain 3
   </td>
   <td>grams
   </td>
  </tr>
  <tr>
   <td><em>Strain(4)</em>
   </td>
   <td>Weight measured on strain 4
   </td>
   <td>grams
   </td>
  </tr>
  <tr>
   <td><em>TarePeriod</em>
   </td>
   <td>Time between automatic zeros (load is lifted from strain gauges and output signal taken as zero mass)
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><em>err</em>
   </td>
   <td>Used during tare to make sure values are stable
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><em>TareCount</em>
   </td>
   <td> Each time a tare occurs, TareCount is incremented by 1. The current value is stored in each data record. Makes it easy in R to use the values close to a tare event.
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><em>TareNow</em>
   </td>
   <td> Is a Boolean (`true` or `false`) flag either set by the code at each tare period or manually set `true` to force a tare.
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><em>autozero</em>
   </td>
   <td>if `true` the tare function is active, if `false` it is not.
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><em>SetPointRH</em>
   </td>
   <td>Desired Relative Humidity, calculated from SetPointVPD and SetPointT.
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><em>SetPointT</em>
   </td>
   <td>Desired Temperature 
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><em>SetPointVPD</em>
   </td>
   <td>Desired vapor pressure deficit
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><em>SetPointAbsH</em>
   </td>
   <td>Desired absolute humidity, calculated from SetpointVPD and SetPointT
   </td>
   <td>grams
   </td>
  </tr>
</table>

## Setting up the graphs

+ Go to the Graphs tab --> Select a graph (Graph 1, Graph 2 or Graph 3)

	[insert image]

+ Press the right click over a empty cell located in the Selected Fields  then select Add..

	[Insert image]

+ Click over the Public tab. A list of variables should appear at the right hand side. 

	[Insert Image]

+ Select one variable and then click Paste

	[Insert image]
