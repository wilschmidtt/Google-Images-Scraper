# Google Image Scraper
Search Google Images for user-defined term(s) and download the first 'x' images to your local machine. Useful for generating the seed images needed for training an image classifier

### Example Run

![images](images/image_scraper.gif)

##### Breif Explanation:
Search Google Images for the term 'cat' and download the first 50 images to appear, then search Google Images for the term 'dog on grass' and download the first 50 images to appear. All images are automatically saved into a folder titled 'google_images', and the images for each search term are saved into the 'cat' and 'dog_on_grass' folders respectively. All images are then converted to .jpg

### Prerequisites
* Python 3.7.*
   - Any version of Python 3.7 will work 
   - The 'requirements.txt' file contains all of the necessary libraries. It is recommended that you install them onto a fresh environment
   
### image_scraper.py Explained
* The program sends a request to Google Images, along with whatever term(s) you entered, and waits for the dynamically loaded source code to be returned
* Once the source code has been returned, the program parses it and extracts 'x' number of images, with 'x' being entered by the user
* Images for each term will be saved into whatever working directory you are using, with a folder being created f or each respective term

### Running the image_scraper
* Once you have set up the environment, navigate to the directory where you have saved the program and run: ```$ python .\image_scraper.py -h```
* There are two commands that need to be supplied prior to running the program. They are as follows:
    * -m MAX_IMAGES, --max_images MAX_IMAGES
           - max number of images to scrape, default set to 20
    * -t SEARCH_TERMS [SEARCH_TERMS ...], --search_terms SEARCH_TERMS [SEARCH_TERMS ...]
           - terms to search for
### Inspiration
* Wanted to create an easier way to collect the seed images that are used as the basis for training an image classifier

### Author
* **William Schmidt** - [Wil's LikedIn](https://www.linkedin.com/in/william-schmidt-152431168/)
