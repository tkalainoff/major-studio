# Qualitative Project

## Initial Concept Sketch
![Sketch_1](https://user-images.githubusercontent.com/77869514/196469786-e8bfdc72-358c-4f78-a56b-34eea7d2d809.jpg)

## Data Source + Review
https://www.unhcr.org/refugee-statistics/download/?url=2z1B08

<img width="1420" alt="Screen Shot 2022-10-18 at 12 11 17 PM" src="https://user-images.githubusercontent.com/77869514/196485780-6ba7bbb4-507f-40c0-b03f-578a16909267.png">

## Data Cleaning and Restructuring
https://observablehq.com/d/829a66acf746a618

```json
{
  "source": "Afghanistan"
  "target": "Albania"
  "value": 5
}

{
  "source": "Albania"
  "target": "recognized"
  "value": 5
}

{
  "source": "Austria"
  "target": "protected"
  "value": 1730
}

{
  "source": "Australia"
  "target": "rejected"
  "value": "28"
}

{
  "source": "Armenia"
  "target": "closed"
  "value": "5"
}
```

## Code Prototype
<img width="659" alt="Screen Shot 2022-10-15 at 1 20 27 AM" src="https://user-images.githubusercontent.com/77869514/196485779-cf02db52-0255-4e87-82aa-03cc90b60956.png">

Using the guided code from here: https://bl.ocks.org/d3noob/06e72deea99e7b4859841f305f63ba85 I was able to use some test data and input into this sankey diagram

Below is an attempt to input the more comprehensive dataset and I broke it :( 
<img width="639" alt="Screen Shot 2022-10-15 at 1 19 30 AM" src="https://user-images.githubusercontent.com/77869514/196485776-6b21ccc5-bb2c-4402-86d1-e3d1dbce85e8.png">

The next challenge will be to edit the code to accomodate for more data

<img width="1247" alt="Screen Shot 2022-10-25 at 11 17 47 PM" src="https://user-images.githubusercontent.com/77869514/197926674-b6d29462-ca55-4537-a1e6-9848d29d6408.png">

The next iteration will work to fine tune the color palette and hover on effects to improve clarity of the visualization. Also, so reworking of numbers to ensure that all the nodes across the three sections ultimately add up to the same height.

<img width="1042" alt="Screen Shot 2022-11-01 at 12 09 44 PM" src="https://user-images.githubusercontent.com/77869514/199387047-cf5b9796-fa5c-48f4-b851-445b1551b1fd.png">

<img width="1023" alt="Screen Shot 2022-11-01 at 11 15 46 PM" src="https://user-images.githubusercontent.com/77869514/199387330-386e9508-f3fa-4b99-803d-f05640f47469.png">

## Design Mockup 

https://www.figma.com/file/r6tn3xB6eOOYMJwCDoUs0w/Asylum-Sankey?node-id=0%3A1
https://www.figma.com/community/plugin/991975059967102509/Sankey-Connect

In order to make a design mockup and fimga I played around with my data in excel to make some manual calculations that would be necessary to accurately create proportional nodes. Below is a screenshot of those calculations: 

<img width="1076" alt="Screen Shot 2022-10-25 at 9 22 19 AM" src="https://user-images.githubusercontent.com/77869514/197786236-9ec6aa8d-20c5-4dda-a41c-c8426334a7a5.png">

The main discovery from this process was that the data of many countries is negligible in comparison/proportion to other countries. So from my first restructuring of my data, I was left with 65 unique countries with data, after these calculations I am left with 19 unique countries with significant amounts of data and one container called "other" to encompass the collection of countries with negligible data.

Though this merging of countries into one container called "other" makes sense for this sankey diagram it does feel dissmissive as each of these data points represent an actual person seeking safety, this adds to the case of having an animated particle sankey diagram where each data point would be a particle moving through the sankey diagram from node to node.

Below is a screenshot of the beginning of a mock up:
<img width="905" alt="Sankey_Mockup" src="https://user-images.githubusercontent.com/77869514/197786223-23eff82c-f149-428b-97ec-cfba04ddf4dc.png">



