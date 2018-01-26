# Advance Lane Finding Project
Marking the lane boundaries and area in front

Started the project by calibrating camera with the sample images provided. 

Second step was to generate a binary image where lanes alone are visible. This seemed easy but soon found out to be very challenging when we consider images with shadows and extreme day light. It took lot of iterations and utlimatley found a way to integrate 'l' from hls space to get an image that can marked lanes in images which has shadow.

Third step was to get the correct perspective. This again was not easy. I had to settle with manaul coded numbers and not so optimal output. I decided to move on after reading in forum most of us had the same issue.

Fourth step was to find the polynomial. Going for 11 frames and polyfit method did a good job in defining the curve the lanes are taking. Used the best fit polynomial numbers obtained to calculate curvature and center calculation. For curvature I happen to take average of left and right lane and for Center 

Improve on:
1. Identifying lanes during extreme day light or snow on the sides of road or road full of shadow
2. Work on challange videos
Further Read :
1. Curvature & Center calcuations
2. Convolution Method
