# ImageViewerApp
This is an android image viewer application with limited functionality.

STEP 1:
I set up the look and feel for the android image viewer application which will consist of adding an android ImageView to the android RelativeLayout and then accessing the android ImageView from the android RelativeLayout inside code in the activity.

STEP 2:
I introduced android intents and used the functionality of the available  images.

STEP 3:
I introduced the onActivityResult method and showed how it can be used to get information back from any requests made from our application intents. The information we will be looking for in this particular case is the Uri which references the location of our image.

STEP 4:
I created an android image viewer using the android local storage framework that was introduced in android lollipop.

STEP 5:
I highlighted two major issues with the current android image viewer application and identify various solutions to rectify those problems. The solution I choose for this is the Glide image loading library.

STEP 6:
I added a long click listener to the image. When a finger is placed and held on the image it will activate the long click listener and display a toast message.

STEP 7:
I created our own custom ImageView which is basically our own class which extends from the android ImageView class.

STEP 8:
I added an animation for expanding the thumbnail into the full size image.

STEP 9:
I used the custom image view's ondraw method to display the bitmap. This is in preparation for setting the pinch zoom implementation.

STEP 10:
I specified the dimensions of the image view using the custom view's onMeasure method. This is important for the image viewer application because the original image may only take up a portion of the display but in the zoomed in state you may want to use all of the available screen real-estate available so the image view dimensions and size will change depending on the zoomed state.

STEP 11:
I zoomed in and out of the image using the two finger pinch technique. Note that there will be no panning implemented yet. Just the pinch & zoom.

STEP 12:
I implemented panning when the image has been zoomed in. I focused on setting up the initial touch listeners for image panning. There are two issues that needed to be resolved. The boundary limits of the bitmap are not enforced and the previous panning coordinates are not saved.

STEP 13:
I saved the location from the previous pan and then set panning limits which match the boundary of the image.
