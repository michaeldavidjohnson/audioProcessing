Potential ways to fix the FPS issue:
  - Moving to pyqtgraph
  - figuring out a way to remove the canvas.draw() from MatPlotLib, we should just re-draw the lines, especially as the plots
    don't even have an axis. Doing this change could *substatially* increase the frame rate.
    
    
    
This is of high importance. If the fps is really high then we can increase the time.sleep() to a desired frame rate. This should
substantially reduce CPU usage and would make it pretty safe to start using in daily life.
