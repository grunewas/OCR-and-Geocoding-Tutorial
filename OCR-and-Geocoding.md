# Optical Character Recognition (OCR) and Geocoding Tutorial
Susan Grunewald

This little tutorial will show you two different methods to turn a PDF image file into text. Most PDF files are scans of text in which the text is rendered as a picture file and not editable text. The first step you need to do is to perform optical character recognition, or OCR, to turn the pictures into text that can then be modified. There are different open source OCR web based platforms that you may wish to use depending on the format of your text. If you text is in paragraph form, use the first one. If you text is in tabular format, that is it is in a table layout, use to the second.

Once your information has been converted to text, you can run it through a variety of different other web services to geolocate place names in the text to create maps from it.

## Optical Character Recognition (OCR)

### OCR of Paragraph Text

Take a PDF document that is text in paragraph form.
 - Go to [Free Online OCR Service](https://www.onlineocr.net/).
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
 -  Wait for the upload to process and then double click on the title of the file you uploaded.
 -  You will see the text of your file. It has been automatically annotated by the software. Read through the text to see if it highlighted all of the correct locations.
 -  Click on the highlighted locations to see where it has mapped them. Make sure that it has found the correct instance of a place name. For example, if you are studying Soviet history and need to locate and map Brest, make sure that you double check that it has selected Brest, Belarus and not Brest, France.
 -  At the top of the screen, click the Map View icon to open the map and see the visualization of the places mentioned in your text. You can export these geometries for use in other mapping programs by clicking Download Options at the top. Keep in mind that you might have to reformat the export data for other mapping software.

### Finding Places with an Online Service
If you only have a few locations to look up, it is easy to type each location into Google Maps, right click on a spot on the map, and then click "What's Here" to have a new window open up with latitude and longitude coordinates that you can copy and paste into a spreadsheet for use in mapping software. If you have up to 100 locations that you want to look up at once, use the following steps.
 - Open [Google Map Developers Batch Geocode Tool](https://www.mapdevelopers.com/batch_geocode_tool.php).
 - Paste up to 100 locations in the box.
 - Click "Find Addresses" below to run the service.
 - Copy and past the locations it found into a spreadsheet for use with mapping software.
 - Manually look up locations it could not find in Google Maps or with other geographic reference authorities such as the [Getty Thesaurus of Geographic Names (TGN)](http://www.getty.edu/vow/TGNFullDisplay?find=brest&place=&nation=&prev_page=1&english=Y&subjectid=7017021).
