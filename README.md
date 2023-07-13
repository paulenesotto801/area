# area
/**
 * Calculates the area of a rectangle.
 * 
 * @param {number} length - The length of the rectangle.
 * @param {number} width - The width of the rectangle.
 * @returns {number} The area of the rectangle.
 */
function calculateArea(length, width) {
  try {
    // Check if both arguments are numbers
    if (typeof length !== 'number' || typeof width !== 'number') {
      throw new TypeError('Both arguments must be numbers');
    }
    
    // Calculate and return the area
    return length * width;
  } catch (error) {
    // Log the error
    console.error('Error:', error.message);
    return 0;
  }
}
