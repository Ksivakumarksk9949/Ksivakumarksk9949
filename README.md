<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Responsive Portfolio</title>
<style>
  :root {
    --primary-color: #4CAF50; /* Primary color variable */
    --transition-speed: 0.3s; /* Transition speed variable */
  }

  body {
    margin: 0;
    font-family: Arial, sans-serif;
  }

  /* Flex container for the portfolio items */
  .portfolio {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 10px;
    padding: 10px;
  }

  /* Portfolio item */
  .item {
    flex-basis: calc(33.333% - 20px);
    border: 1px solid #ddd;
    padding: 10px;
    transition: transform var(--transition-speed);
  }

  /* Hover effect for portfolio items */
  .item:hover {
    transform: scale(1.05);
    border-color: var(--primary-color);
  }

  /* Responsive media query */
  @media (max-width: 800px) {
    .item {
      flex-basis: calc(50% - 20px);
    }
  }

  @media (max-width: 500px) {
    .item {
      flex-basis: 100%;
    }
  }
</style>
</head>
<body>

<div class="portfolio">
  <div class="item">Item 1</div>
  <div class="item">Item 2</div>
  <div class="item">Item 3</div>
  <!-- Add more items here -->
</div>
