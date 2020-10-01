# Open Process Imaging
This is a page for sharing an open process for digitizing film negatives using a DSLR and macro lens. You can use this process to scan your own negatives, or you can use your equipment and expertise to scan for others.

I used the term _Open Process_ because it is similar to _Open Source_ except instead of computer source code it's a technical process that's being shared. There is actually a lot of information on how to do this, but I wanted to include some additional process for people who want to take this and maybe do a bit of side hustling for friends and acquaintances in your neighbourhood.

The technology exists to 'scan' colour and B&W negatives quickly and with very high quality using a digital SLR camera and a good macro lens. Scanning negatives (often quite old negatives) has historically been challenging because even if you had access to a good quality scanner it takes a very long time. Once you get the scan it takes another very long time to get the colours and tones to an acceptable state. With recent software like Negative Lab Pro (an Adobe Lightroom Plugin) this is made much faster and simpler.

Taking a picture of the negative with a good macro lens and SLR camera means that you can get images that are nearly the full resolution of the camera's sensor. In my case I use a camera with an 18MP sensor; nearly all of that is dedicated to capturing the negative. As a result, the final image is nearly a full 18MP, more than a standard (non-pro) lab would give with their scans. Additionally, you will shoot the image in RAW format which gives a lot of flexibility for adjusting the colours and cropping as you need.

A high quality macro lens is essential for this process. You want one that has a 1:1 ratio, meaning the lens can focus close enough so that an object 35mm across fits across the entire camera sensor. There is no scaling up needed for a 35mm negative scan; it is all completely optical enlargement.

# Equipment List
For those of you who want to do this yourselves there are lots of resources online but here is a quick list of the equipment I use right now, in case you want to copy my process:
1. Canon T3i digital SLR camera
2. Canon 100mm f/2.8L IS macro lens
3. Manfrotto MKC3-H01 tripod (with center post that can be inverted, very important)
4. Smartphone to use as backlight for the negatives (set to full brightness for scanning)
5. Homemade negative holder (out of Lego!) to hold the negatives securely a few cm above the backlight
6. Adobe Lightroom Classic (part of Adobe Creative Cloud subscription)
7. Negative Lab Pro plugin - essential for getting excellent colours out of the orange negative scans
8. Computer - obviously to run Lightroom but also to remotely control the camera shutter via USB
8. Random things like an air dust blower, gloves, tweezers for grabbing negative strips from tight holders

You could likely get set up with all the hardware you need (used) for less than $1000. Adobe Creative Cloud is an additional $15/month, and Negative Lab Pro is $100 USD (perpetual license). This isn't all that bad especially if you already have some of the equipment. For those who do not have the equipment, I'd like to see a network of local friends who would be willing to scan others' negatives for a small fee. I have a suggested fee structure below for those who want to maybe do this for others - it is not lucrative but it is enough of an incentive to make it worthwhile.

# Obvious Improvements
Some equipment improvements would likely help with efficiency, and likely with overall quality of the scans. Thankfully for me the biggest factor is the macro lens; there are no improvements I need to make in that area. However, others are:
1. Canon T3i --> [Canon EOS RP](https://www.canon.ca/en/product?name=EOS_RP&category=/en/products/Cameras/Mirrorless-Cameras) Mirrorless Full Frame camera body. Not a huge increase in MP but would improve ease of use for sure and may squeeze out a bit of extra detail from very high quality negatives.
2. Smartphone backlight --> [Skier Copy Box](http://skier.com.tw/web/shop/shop_in.jsp?pd_id=PD1599461016799) backlight and negative holder. This would also replace the (admittedly awesome) Lego holder. This is the first upgrade I would like to tackle as it would have probably the most direct impact on final image quality due to the fact that the light is brighter and gives better colour reproduction. There are other options for backlights but if they're cheaper they're not worth getting, and if they're more expensive they're _a lot_ more expensive!
3. Manfrotto tripod --> [Copy stand](http://skier.com.tw/web/shop/shop_in.jsp?pd_id=PD1600329566638). This is not going to give any improvement to image quality but would make setup and alignment an awful lot easier.

# The Process
## Folder Structure
* Main folder of "Scans" which contains everything inside it.
* Subfolders "Personal" and "Others"
* In "Others", a folder for each person's scans. This could be in the format Lastname_ID, where the _ID suffix is a 3-digit zero-padded integer starting at 0. This becomes the full person ID. The details of the person are recorded (currently) in an Excel or Google Sheets workbook so they can be looked up if necessary.
* The folder structures of "Personal" and each person's individual folder are identical.
* Inside each person's folder there is a folder for each scan job. Each job has an ID, which is the date (yyyy_mm_dd) that the job was created, prefixed with "JOB_". 
* Inside each scan job folder there is another folder for each negative "group". This could be a negative sheet (like mine) from a binder, it could be a negative sheet from the photo developer (those folded sheets that come inside the Costco photo envelopes along with the prints), or it could be some other thing like a box. However it has been organized originally is how it will be organized in the folder structure. Ideally this should closely correspond to a single roll of film.
    * The group ID is "GRP_" plus a numeric identifier (3-digit zero-padded integer starting at 1 inside each job folder). This will correspond to a note placed with the group of negatives, either written on the sheet or provided as a sticky note or other paper affixed to the group.
    * Someone might have already given their groups IDs in which case we will just use those (as long as they're unique, may need a numeric suffix otherwise).
    * If a group is large (like a box of unsorted negatives), and if the person doesn't have any other way of organizing, then the negatives will be arbitrarily sorted into groups of 7 negative strips. If it is a negative roll, this will be its own group obviously (though I don't have a good way of scanning rolls without them curling, and I have a hard time keeping them from being scratched). Maybe negative rolls will be not something I should do right now, until I can get proper equipment for that (if ever). If I group negatives myself I'll have to put each grouping into its own paper sleeve after scanning.
    * The individual strips will not be in their own folders, as that will be too onerous to navigate later on. However, a 'strip number' should be put into the metadata numbered from 1 to nn, usually to 7, from top to bottom based on the orientation of the group itself. If the group has no orientation (loose collection of negative strips for example) this will just be the order that they were scanned.

Metadata for the image could include the frame number, job number, group number, strip number, plus any other information we can get from the film itself such as brand, ISO, etc. This may be unnecessary information, TBD.

## The Steps
### Initial Setup
1. Clear off the work surface
2. Turn off overhead lights (most lights in the room actually)
3. Have batteries fully charged (unless using an AC adapter)
4. Set up tripod and scan table
5. Plug camera in to computer
6. Have handy the air blower and anti-static brush and gloves and tweezers

### At the Start of a Job
1. Create a folder inside Scans for the person, if not already there
2. Add person record to the Excel/Google sheets workbook with their details and ID
3. Create a folder inside Scans for the job
4. Add job record to the Excel/Google sheets workbook with the job details
5. Create an INFO.txt file inside the job folder with details of the job, if provided. Otherwise just the job ID and date. Perhaps start date and completion date.
6. Have a pen / pencil / sharpee / whatever ready
7. Have sticky pad ready in case group ID needs to be written on it
8. Plug in and turn on light source
9. Place negative holder over light source
10. Using a test negative strip set up the placement and height of the negative holder to maximize the area of the frame, while leaving a small amount of border for white balance control.
11. Set camera to autofocus, ISO 100 (or lowest), and f/8 aperture priority. Ensure exposure is set to middle (not over/under) and no additional in-camera settings like saturation etc. (all neutral).
    * TBD on the exposure settings. It may be better to use +1 exposure, and may also be better to use identical exposure for all frames instead of using aperture priority. Need to do some tests on that.
12. Test focus with the test negative strip, and remove the test negative strip. If a shot was taken, delete the test shot from the group folder.

### At the Start of a Group
1. Create folder inside the job for the group
2. Create an INFO.txt file inside the group folder with any metadata (description) of the group. This could include details about who processed the film, on what date, etc. Details that are on the sticker from the developer if it's in one of those paper envelopes. Maybe taking a photo of the picture is sufficient, and saving it inside the group folder? Would be nice to add this information to the image metadata though.
3. Open EOS remote capture and set the target save folder to be the new group folder
4. If there are no groups (big ol' box of negatives), grab 7 strips as a group. If this is done make sure there is an envelope or something else to put the negatives into, to designate them as groups for the person.

### For Each Strip 
These should be strips of 2 frames or more only, not sure how to do individual negative frames but could maybe be the same way, depending on the negative holder?
1. Put on gloves
2. Grab negative strip from group (sheet, loose, whatever)
3. Blow dust off with blower
4. Wipe with anti-static brush (maybe overkill if using the blower)
5. Insert strip into negative holder, emulsion side up
6. Focus and confirm placement of negative frame
7. Take shot
8. Move to next frame and repeat for each
9. Remove strip from negative holder and place back into the sheet (or wherever it came from)

### At End of Group
1. Mark the group id on the group (either sticky note, writing on the group page itself, etc.)
2. Go back to 'At start of group' section if scanning more groups

### When Scanning is Complete
1. In Lightroom, select all the scans and mirror them (since the scans were done emulsion side up)
2. Work magic with Negative Lab Pro, colours and tone balancing! And maybe some manual dust removal.

# Proposed Fee Structure
If you want to do this for others, here's a very basic fee structure to use as a baseline. This tries to stay somewhat close to other alternative scanning services (like those that send offshore) but will necessarily be a little bit higher. Compensating for this is the (proposed) practice of working very locally and picking up negatives from folks in person, then delivering them back when they're complete.

Generally there should be a $5.00 minimum charge to avoid the hassle of having to scan a single strip of 4 negatives for a buck.

_However_, I suggest providing a free strip of 4 negatives to people who are curious about what the quality might be like. This should be with the full scan service to illustrate the quality of the process and let them decide whether it's worth them spending more money to get a bunch of rolls digitized.

## Raw Scanning Service
Raw scans would be done for $0.25 each.

Raw scans are literally just the scanned image. The colours have not been inverted, the white balance has not been set, no cropping has been done. The only processing is mirroring the image in Lightroom because they've been scanned emulsion side up (effectively upside down). These are supplied in the RAW format of your camera. In the case of Canon these will be CR2 files.

This service is suitable for those who are comfortable with image editing software on their own and are happy doing all of the colour inversion and balancing themselves. They may even want to get started with Lightroom and Negative Lab Pro for a smaller financial investment, but they don't want the larger investment of the hardware.

This is pretty good value for that sort of person, with a roll of 24 frames coming in at $6.00.

## Basic Scanning Service
Basic scans are $0.50 each.

Basic scans take the RAW files, white balance, invert, and colour balance them using Negative Lab Pro. This will result in a positive image that is reasonably well colour balanced, though it will probably be a bit flat because no custom colour or tonal balancing will be done on a per-image basis. No cropping will be done on the positive image (giving the person flexibility to crop as they wish).

This service is suitable for those who like to tweak brightness and contrast settings on their own in a basic or advanced photo editor. It also is suitable for those who use Lightroom, Photoshop, or another image editing program but do not want to bother with purchasing and learning how to use dedicated software like Negative Lab Pro. It also would be good for people who want to post photos to Flickr or Instagram or somewhere else, and apply creative filters from those platforms along the way.

In addition to the negative-image RAW files, positive-image TIF files are delivered.

## Full Scanning Service
Full scans are $1.00 each.

This takes the basic scans and adds custom colour balancing, tonal balancing, cropping, and some manual dust removal. The result of these scans should be images that are colour accurate and have good pleasing tonal range. They are supplied as cropped and rotated JPG files suitable for posting, emailing, printing, or what have you.

In addition to the JPG files, the negative-image RAW files, and flat positive-image TIF files are delivered. There is another TIF file delivered which matches the edits made before the final JPG conversion. This is 4 images altogether.

This can be pretty time consuming but it is correspondingly expensive.