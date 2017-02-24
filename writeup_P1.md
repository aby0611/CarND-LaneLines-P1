#**Finding Lane Lines on the Road** 

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report

---

### Reflection

###1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 6 steps.  

1. Define color_thresholds for obtaining the boolean matrix to identify pixels below the thresholds.

2. Find the region inside the lines and then identify region_thresholds based on the lines.

3. Covert the image to grayscale.

4. Getting Canny edges.

5. Run Hough on edge detected image.

6. Draw the lines from Hough edge detecyed image if it's contained in region_thresholds of step 2.

###2. Identify potential shortcomings with your current pipeline

One potential shortcoming would be the white lane is not clear while while the length of white lane is long.

###3. Suggest possible improvements to your pipeline

I think I need to do more experiments for making the wirte line detection more precious while the length of white lane is long. Maybe doing some improvement on  using GaussianBlur function.