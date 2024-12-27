Expanding Cards

Expanding Cards is a visually appealing interactive component built using HTML, CSS, and JavaScript. This project features a set of panels that expand and collapse when clicked, providing a clean and intuitive user interface for showcasing content such as images or descriptions.

Features

Smooth animation for expanding and collapsing panels.

Fully responsive design, adapting to different screen sizes.

Modern typography and styling.

Lightweight and simple implementation.

Demo

A live demonstration of this project can be accessed at [your live link here, if applicable].

Technologies Used

Languages and Tools:

HTML: Structure of the panels and headings.

CSS: Styling for the layout, animations, and responsive behavior.

JavaScript: Adds interactivity to the panels.

How It Works

HTML Structure: Each panel is wrapped in a container and styled with background images and headings.

CSS Animations: Transitions are applied to panels and headings for smooth resizing and fading effects.

JavaScript Interaction: Panels toggle the active class when clicked, dynamically resizing and showing their content.

Installation and Setup

Clone the Repository

# Clone this repository
git clone https://github.com/workout33/expanding-cards.git

# Navigate into the directory
cd expanding-cards

Open Locally

Open the index.html file in any modern web browser to view the project.

File Structure

Expanding Cards
├── index.html   # Main HTML file
├── style.css   # Stylesheet for layout and animations
└── script.js   # JavaScript for interactivity

Usage

Click on any panel to expand it. Other panels will automatically collapse.

Titles appear when a panel is expanded, enhancing readability and user experience.

Responsive Design

Panels dynamically adapt to different screen sizes.

On screens smaller than 480px, the last two panels are hidden for better usability.

Code Highlights

HTML

<div class="container">
  <div class="panel active" style="background-image: url('image1.jpg')">
    <h3>Title 1</h3>
  </div>
  <!-- Additional panels -->
</div>

CSS

.panel {
  flex: 0.5;
  transition: all 0.8s ease;
}

.panel.active {
  flex: 5;
}

JavaScript

const panels = document.querySelectorAll('.panel');

panels.forEach(panel => {
  panel.addEventListener('click', () => {
    removeActiveClasses();
    panel.classList.add('active');
  });
});

function removeActiveClasses() {
  panels.forEach(panel => {
    panel.classList.remove('active');
  });
}

Contributing

Contributions are welcome! Feel free to fork this repository and submit pull requests.

License

This project is licensed under the MIT License. You are free to use, modify, and distribute this project as long as you include the original license.

Acknowledgments

Unsplash: For providing the beautiful images used in this project.

Google Fonts: For the modern typography (Muli font).

Author

@WORKOUT
