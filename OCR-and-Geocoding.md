# Optical Character Recognition (OCR) and Geocoding Tutorial
Susan Grunewald

Updated: 10/3/2019

This little tutorial will show you two different methods to turn a PDF image file into text. Most PDF files are scans of text in which the text is rendered as a picture file and not editable text. The first step you need to do is to perform optical character recognition, or OCR, to turn the pictures into text that can then be modified. There are different open source OCR web based platforms that you may wish to use depending on the format of your text. If you text is in paragraph form, use the first one. If you text is in tabular format, that is it is in a table layout, use to the second.

Once your information has been converted to text, you can run it through a variety of different other web services to geolocate place names in the text to create maps from it.

## Optical Character Recognition (OCR)

### OCR of Paragraph Text
These steps are for a simple online service that isn't great. One of the best OCR programs is from the paid version of Adobe Acrobat. If you have that through a university or your own personal subscription, great. Use that. Follow the steps [here](https://acrobat.adobe.com/us/en/acrobat/how-to/ocr-software-convert-pdf-to-text.html) to do OCR with Adobe. For our purposes and for those without Adobe, take the following steps:

Take a PDF document that is text in paragraph form.
 - Go to [Free Online OCR Service](https://www.onlineocr.net/).
 - Create a free account to OCR more than one page of text.
 - Upload the PDF image and tell it to export at a .txt file.

Great. Now the text is ready to edit. You may have to clean a lot of it depending on how good the image was and how good the software was at reading it. Languages other than English often require more cleaning.

### OCR of Tabular Text
 -  Go to [Tabula](https://tabula.technology/) and follow the installation steps
 -  Upload your PDF to Tabula.
 -  Select the different columns or rows of text that you wish to perform OCR on.
 -  Run the program.
 -  Clean your output text as needed.

## Geocoding Place Names From Text

There are numerous programs and websites that will allow you to map locations from place names.

### Finding Places with Recogito
 -  Create an account for [Recogito](https://recogito.pelagios.org/).
 -  Log in and then upload your .txt file to Recogito.
 -  Wait for the upload to process.
 -  Click your text file once to have an options button appear in the top right corner.
 -  Select Named Entity Recognition.
 -  Choose a recognition format (or just use the default) and persom the process.
 -  Double click on the text file name to open it and read the text. It has been automatically annotated by the software. Read through the text to see if it highlighted all of the correct locations.
 -  Click on the highlighted locations to see where it has mapped them. Make sure that it has found the correct instance of a place name. For example, if you are studying Soviet history and need to locate and map Brest, make sure that you double check that it has selected Brest, Belarus and not Brest, France.
 -  At the top of the screen, click the Map View icon to open the map and see the visualization of the places mentioned in your text. You can export these geometries for use in other mapping programs by clicking Download Options at the top. Keep in mind that you might have to reformat the export data for other mapping software.

### Finding Places with an Online Service
If you only have a few locations to look up, it is easy to type each location into Google Maps, right click on a spot on the map, and then click "What's Here" to have a new window open up with latitude and longitude coordinates that you can copy and paste into a spreadsheet for use in mapping software. 
 - Manually look up locations it could not find in Google Maps or with other geographic reference authorities such as the [Getty Thesaurus of Geographic Names (TGN)](http://www.getty.edu/vow/TGNFullDisplay?find=brest&place=&nation=&prev_page=1&english=Y&subjectid=7017021).
 - Microsoft Excel has a Geocoding function as well. Follow the steps [here](https://www.adventuresincre.com/auto-populate-latitude-longitude-excel/) to download and run the latitude and longitude from Google Maps function in Excel.

You can also use a batch geocode service to look up about one hundred locations at a time. Unfortunately, Google Maps updated their API any many of the webservices that did this type of work are now borken. You can still use [this service](https://www.gpsvisualizer.com/geocoder/) but first you need to follow the steps from [this website](https://developers.google.com/maps/documentation/javascript/get-api-key) to get an API key for Google Maps to use with the web service. 
