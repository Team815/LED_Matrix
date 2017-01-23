# LED_Matrix
Code for an LED_Matrix

Reference

Create the matrix
	RGBmatrixPanel matrix(A, B, C, D, CLK, LAT, OE, false, 64);

Start the matrix (in setup)
	matrix.begin();

Draw a white pixel in the top-left
	matrix.drawPixel(0, 0, matrix.Color333(7, 7, 7)); 

Draw an 8x10 red filled rectangle
	matrix.fillRect(0, 0, 8, 10, matrix.Color333(7, 0, 0));

Draw a green hollow rectangle around the border
	matrix.drawRect(0, 0, matrix.width(), matrix.height(), matrix.Color333(0, 7, 0));

Draw a blue line from the top left to the bottom-right
	matrix.drawLine(0, 0, matrix.width()-1, matrix.height()-1, matrix.Color333(0, 0, 7));

Draw a yellow hollow circle
	matrix.drawCircle(10, 10, 10, matrix.Color333(7, 7, 0));

Draw a violet filled circle
	matrix.fillCircle(40, 21, 10, matrix.Color333(7, 0, 7));

Fill the screen with black
	matrix.fillScreen(matrix.Color333(0, 0, 0));

Text functions
	matrix.setTextSize(1); // size 1 == 8 pixels high, size 2 == 16 pixels high
	matrix.setTextWrap(false);
	matrix.setTextColor(matrix.Color333(7,7,7));
	matrix.setCursor(0, 0);
	matrix.println("LED MATRIX!");