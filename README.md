# Week 1 - Day 3: Advanced HTML & Multimedia

## Topic
HTML5 forms validation, audio/video tags, iframes, and tables for data.

## Learning Objectives
- Create accessible HTML forms with built-in validation.
- Embed audio and video using HTML5 tags.
- Use iframes safely for external content.
- Build readable data tables with proper structure.

## Warm-Up Review (5 minutes)
Quick questions:
- What is a semantic tag?
- Why use `article` or `section` instead of `div`?
- What does `main` represent?

## HTML5 Forms + Validation (15–20 minutes)
**Key ideas:**
- Use proper input types for better validation and mobile keyboards.
- Required fields help prevent empty submissions.
- Labels improve accessibility.

**Example form:**
```html
<form>
  <label for="name">Full Name</label>
  <input id="name" name="name" type="text" required />

  <label for="email">Email</label>
  <input id="email" name="email" type="email" required />

  <label for="age">Age</label>
  <input id="age" name="age" type="number" min="10" max="80" />

  <label for="site">Portfolio</label>
  <input id="site" name="site" type="url" placeholder="https://example.com" />

  <button type="submit">Submit</button>
</form>
```

**Teacher notes:**
- `required` makes a field mandatory.
- `type="email"` checks format automatically.
- `min` and `max` restrict number inputs.

## Audio & Video Tags (10–15 minutes)
**Audio example:**
```html
<audio controls>
  <source src="audio/sample.mp3" type="audio/mpeg" />
  Your browser does not support the audio element.
</audio>
```

**Video example:**
```html
<video controls width="480">
  <source src="video/demo.mp4" type="video/mp4" />
  Your browser does not support the video tag.
</video>
```

**Teacher notes:**
- Always include controls so users can play/pause.
- Provide fallback text for unsupported browsers.

## Iframes (10 minutes)
**Example (YouTube embed):**
```html
<iframe
  width="560"
  height="315"
  src="https://www.youtube.com/embed/dQw4w9WgXcQ"
  title="YouTube video"
  allowfullscreen
></iframe>
```

**Teacher notes:**
- Use iframes only for trusted sources.
- Provide a title for accessibility.

## Tables for Data (15 minutes)
**Example table:**
```html
<table>
  <caption>Student Scores</caption>
  <thead>
    <tr>
      <th>Name</th>
      <th>HTML</th>
      <th>CSS</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Ayesha</td>
      <td>85</td>
      <td>90</td>
    </tr>
    <tr>
      <td>Ali</td>
      <td>78</td>
      <td>82</td>
    </tr>
  </tbody>
</table>
```

**Teacher notes:**
- Use `th` for headers.
- Use `caption` for accessibility.

## Practical Lab: Multimedia Webpage (20–30 minutes)
**Task:** Build a single HTML page that includes:
- A form with at least 3 fields and validation.
- One audio element.
- One video element.
- One iframe (map or YouTube).
- A table with at least 3 rows.

**Starter structure:**
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Multimedia Page</title>
  </head>
  <body>
    <h1>My Multimedia Page</h1>

    <h2>Contact Form</h2>
    <!-- Add your form here -->

    <h2>Audio</h2>
    <!-- Add your audio here -->

    <h2>Video</h2>
    <!-- Add your video here -->

    <h2>Embedded Content</h2>
    <!-- Add your iframe here -->

    <h2>Data Table</h2>
    <!-- Add your table here -->
  </body>
</html>
```

## Wrap-Up (5 minutes)
Quick questions:
- Which input type checks email format?
- Why add a caption to a table?
- When should you use an iframe?

## Homework (optional)
Create a "Student Profile" page that includes:
- A validated form.
- One audio or video.
- A table of skills and scores.
