# MO Stay

![image](files/logo4.png)

Get MO Stay availability up to the next two months.

![image](files/demo.gif)

[View the source code](https://github.com/m-soro/mostay/blob/main/mostay)

[Visit Mandarin Oriental Website](https://www.mandarinoriental.com/)

This project was created to make it easier for me to check MOstay availabilities. Although, Mandarin Oriental's website is beautiful and intuitive. The brand has many popular properties all over the world and is not always available for MOStay bookings. 

I built this program using the Selenium and Pillow packages. Selenium is used for browser automation and Pillow is used for screenshot/image processing. 

To create this project, I had to do the following:

1. Visit the reservation page complete with:
    * Correctly formatted date
    * Property idetifier
    * MOStay code
   The other data from the URL are optional. I found this out by testing what is the least info needed to return what I was looking for.

2. Take the screenshot calendar screenshot.
   I found the element that I needed to screenshot using the inspect option from my browser and using Selenium to select the element.
   
3. Simulate a click to view the next image and take a screenshot.
   MOStay availabilities can only be viewed for the following two months. This action has to be done twice.
   
4. Take screenshot of the property name.

5. Concatenate all of this images.
   I have to first stitch all of the calendar images, then attach the property name image. This is accomplished by Pillow package.  

In detail:

To start I needed to create a dictionary of all Mandarin Oriental property name and their respective hotel code. This data can be found in the hotel selection dropdown by using the ispect tool. To keep the focus on this program, I saved this dictionary on a separate .py file and imported it to my main program. 

Next, I have to construct the URL with all the data needed to produce the correct hotel's calendar image. Using the input from my terminal, by giving three letter or if neccessary the whole location name (if location name) are very similar. I should be able to look for the closest match in my dictionary. 

After the successfully prio

 
