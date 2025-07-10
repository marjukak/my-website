Task: Personal Portfolio Web Page
For this task, I was asked to create a personal website that showcases my basic information, fun facts, hobbies, and a bit of personality. I decided to go with a clean and minimalistic design while making it visually modern and easy to read.
Tools I Used:
Visual Studio Code – My go-to editor for writing and previewing code.
HTML & CSS – The foundation for structuring and styling the website.
Google Fonts – To add a nice modern font (Poppins).
My own profile photo – To give it a more personal and finished look.
What I Built:
The website is a single-page layout that centers a card-like container on the screen. I used Flexbox to align everything both vertically and horizontally. The background has a dark blue gradient that adds a modern touch, while the content box (the container) is white with rounded corners and a shadow to make it pop.
Inside the container, I added:
My name, email, and location
A short "About Me" section
A few fun facts that reflect my personality (yes, including my addiction to egg chicken sandwiches)
My hobbies in a casual and relatable way
And of course, my picture at the bottom to wrap it all up nicely
Styling Details:
I made sure the text was easy to read by choosing good font sizes and spacing. For the fun facts, I added custom bullets using the “⭕” symbol to keep things playful. The image is styled as a circle with a nice blue border to match the overall theme.
Here’s an example of the kind of CSS I wrote:
body {
  background: linear-gradient(135deg, #1e3c72, #2a5298);
  display: flex;
  justify-content: center;
  align-items: center;
}
img {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  border: 4px solid #1e3c72;
}
Reflection:
This task helped me get more comfortable with positioning elements using Flexbox and fine-tuning layouts with CSS. It was also a fun way to present myself through code, and I tried to keep the tone of the content as close to my real personality as possible.


Code:
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>MJ's Personal Website</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      height: 100vh;
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(135deg, #1e3c72, #2a5298);
      display: flex;
      justify-content: center;
      align-items: center;
      color: #fff;
    }

    .container {
      background: rgba(255, 255, 255, 0.95);
      color: #222;
      padding: 40px;
      width: 90%;
      max-width: 800px;
      border-radius: 16px;
      box-shadow: 0 20px 50px rgba(0, 0, 0, 0.2);
      text-align: center;
    }

    h1 {
      font-size: 2.5rem;
      margin-bottom: 10px;
    }

    p, li {
      font-size: 1.1rem;
      margin: 10px 0;
    }

    ul {
      list-style: none;
      padding: 0;
    }

    ul li::before {
      content: "⭕ ";
    }

    img {
      width: 150px;
      height: 150px;
      border-radius: 50%;
      margin-top: 20px;
      border: 4px solid #1e3c72;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Marjuk AK</h1>
    <p><strong>Email:</strong> marjukak987@gmail.com</p>
    <p><strong>Location:</strong> Jeddah, Saudi Arabia</p>
    <p><strong>About Me:</strong> Tech enthusiast, gamer, car lover, and full-time vibing expert.</p>
    
    <p><strong>Fun Facts:</strong></p>
    <ul>
      <li>I once tried to fix my hair and ended up needing a hairdryer with a quiet mode.</li>
      <li>I can get distracted by YouTube and still bounce back like a champ.</li>
      <li>I can eat an egg chicken sandwich and still complain about the service. Priorities.</li>
    </ul>
    
    <p><strong>Hobbies:</strong> Gaming, coding, food hunts, planning luxury dates (yeah, I go all out)</p>

    <!-- Image -->
    <img src="mj.jpg" alt="MJ's Photo">
  </div>
</body>
</html>
