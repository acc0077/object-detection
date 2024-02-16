# object-detection


#### Project Overview
Using Tensorflow to Detect Objects such as people, apples, and cars


#### Project Scope
- The first step was to get Tenorflow's ssd_mobilenet_v2_2 to use for object detection in images.
- The first portion of the project involved looking at the classes of objects the model has the capability of identifying.
- The model gives an output of bounding boxes for the objects, score for the objects, and class of the objects.
- An initial test of using the model to detect an image of me and an apple was successful. The highest scores from the model were for one person and one apple and the bounding boxes matched the image perfectly.
- The second portion was to use the model to identify moving cars in a video.
- To start this portion, I took video data and broke it down into frames of image data so the model could work with it.
- I ran the model on all the frames of the video and specified to only look at objects with class 3 (classes of car) and with a score above 0.2.
- The model performed okay but a good bit more work would needs to be done to be able to productionize this for a task such as counting cars. This is due to a lot of noise in the detected objects and the model's struggles with identifying cars that are darker and have shade next to them.
- A good next step for getting this closer to production would be to slice the images to only get the portions that the model has the most success with identifying cars. Along with this, adding in logic that once a specific car has been identified, the count is taken and the car is not identified again. Doing this and handling of all the noise in the back ground by optimizing the image color, shape, and scores would help this project continue further.


#### Contact Me
- If you are interested in learning more about this project, please contact me at acarterdata@outlook.com.
