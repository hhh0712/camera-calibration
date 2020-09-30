# camera-calibration
opencv camera calibraion
1. config camera_calibration/in_VID5.xml
 盘格的宽度和高度。
<!-- Number of inner corners per a item row and column. (square, circle) -->
<BoardSize_Width>9</BoardSize_Width>
<BoardSize_Height>6</BoardSize_Height>

2. input camera 
 <!-- The input to use for calibration. 
         To use an input camera -> give the ID of the camera, like "1"
         To use an input video  -> give the path of the input video, like "/tmp/x.avi"
         To use an image list   -> give the path to the XML or YAML file containing the list of the images, like "/tmp/circles_list.xml"
         -->
 <Input>"0"</Input>

3. makir build 
   cd build 
   cmake ..
   make

4. Camera_Calibration ../in_VID5.xml