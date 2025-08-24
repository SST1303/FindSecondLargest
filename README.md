# FindSecondLargest
Second Largest Number Finder

A simple web application that finds the second largest number in an array. Built with vanilla HTML, CSS, and JavaScript.

## 🚀 Features

- **Clean & Modern UI**: Beautiful, responsive design with smooth animations
- **Input Validation**: Handles various input formats and edge cases
- **Real-time Results**: Instant calculation and display of results
- **Error Handling**: User-friendly error messages for invalid inputs
- **Cross-browser Compatible**: Works on all modern browsers

## 🛠️ Technologies Used

- **HTML5**: Semantic markup and structure
- **CSS3**: Modern styling with flexbox and transitions
- **JavaScript (ES6+)**: Vanilla JS with modern syntax
- **Responsive Design**: Mobile-friendly interface

## 📱 Screenshots

The application features a clean, card-based design with:
- Input field for comma-separated numbers
- Interactive button with hover effects
- Clear result display
- Modern color scheme and typography

## 🎯 How It Works

The algorithm efficiently finds the second largest number using a single pass through the array:

1. **Initialize**: Set first and second largest to negative infinity
2. **Iterate**: Compare each number with current largest values
3. **Update**: Maintain the two largest numbers during iteration
4. **Return**: Second largest number or null if not found

## 💻 Usage

1. **Open** `index.html` in your web browser
2. **Enter** numbers separated by commas (e.g., `5, 12, 8, 20, 15`)
3. **Click** "Find Second Largest" button
4. **View** the result displayed below

### Example Inputs:
- `1, 5, 3, 9, 7` → Second largest: 7
- `10, 20, 30, 40` → Second largest: 30
- `5, 5, 5, 5` → No second largest (all numbers equal)

## 🔧 Code Examples

### Main Function
```javascript
function findSecondLargest(arr) {
    let first = -Infinity, second = -Infinity;
    for (let num of arr) {
        if (num > first) {
            second = first;
            first = num;
        } else if (num > second && num < first) {
            second = num;
        }
    }
    return second === -Infinity ? null : second;
}
```

### Alternative Approaches
The project includes several alternative implementations in the comments:
- **Sorting Method**: Using array sort and iteration
- **Set Method**: Removing duplicates with Set
- **Reduce Method**: Functional programming approach
- **Two Variables**: Destructuring assignment approach

## 📁 Project Structure

```
second-largest-number/
├── index.html          # Main HTML file
├── style.css           # CSS styles and animations
├── script.js           # JavaScript logic and functions
└── README.md           # Project documentation
```

## 🚀 Getting Started

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- No additional dependencies required

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/second-largest-number.git
   ```
2. Navigate to the project directory:
   ```bash
   cd second-largest-number
   ```
3. Open `index.html` in your browser

### Local Development
- Open the project in VS Code or your preferred editor
- Make changes to HTML, CSS, or JavaScript files
- Refresh the browser to see changes

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

### How to Contribute
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- Built with vanilla web technologies for simplicity and performance
- Inspired by common programming interview questions
- Designed for educational purposes and practical use

## 📞 Contact

- **Project Link**: [https://github.com/yourusername/second-largest-number](https://github.com/yourusername/second-largest-number)
- **Issues**: [https://github.com/yourusername/second-largest-number/issues](https://github.com/yourusername/second-largest-number/issues)

---

⭐ **Star this repository if you find it helpful!**
