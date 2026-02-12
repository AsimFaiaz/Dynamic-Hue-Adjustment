<section id="dynamic-hue-adjustment">
  <h1>Dynamic Hue Adjustment</h1>

  ![Status](https://img.shields.io/badge/status-stable-blue)
  ![License](https://img.shields.io/badge/license-MIT-lightgrey)

  <h2>Overview</h2>
  <p>
    <strong>Dynamic Hue Adjustment</strong> is a single-file HTML demo that explores
    color transformation using HSL (Hue, Saturation, Lightness) calculations.
    It allows real-time comparison between a primary color and a target color,
    while computing the exact hue shift, brightness difference, and contrast variation required.
  </p>

  <p>
    Built entirely with vanilla JavaScript and CSS, this project demonstrates
    how color spaces can be manipulated programmatically without any external libraries.
    It’s ideal for understanding color theory in UI design, theme engines,
    or dynamic styling systems.
  </p>

  <h2>Developer Note</h2>
  <p>
    This project is part of a growing collection of focused mini-demos where I explore
    fundamental programming concepts in clean, self-contained examples.
    The goal is simplicity, clarity, and zero dependencies.
  </p>

  <h2>Key Features</h2>
  <ul>
    <li><strong>Live Color Comparison:</strong> visually compare Primary, Target, and Converted color blocks</li>
    <li><strong>HSL Conversion Engine:</strong> custom <code>hexToHSL()</code> implementation</li>
    <li><strong>Hue Shift Calculation:</strong> displays exact degree difference</li>
    <li><strong>Brightness Adjustment:</strong> shows lightness delta percentage</li>
    <li><strong>Contrast Variation:</strong> compares saturation changes</li>
    <li><strong>Zero Dependencies:</strong> no frameworks, no libraries</li>
    <li><strong>Single HTML File:</strong> easy to copy, modify, or embed</li>
  </ul>

  <h2>How It Works</h2>
  <pre>
  const primaryHSL = hexToHSL(primaryColor);
  const targetHSL  = hexToHSL(targetColor);

  const hueShift   = targetHSL.h - primaryHSL.h;
  const brightness = targetHSL.l - primaryHSL.l;
  const contrast   = targetHSL.s - primaryHSL.s;
  </pre>

  <p>
    The system converts both selected colors from HEX to HSL,
    then calculates the mathematical delta between their values.
    This gives insight into how much transformation is required
    to morph one color into another.
  </p>

  <h2>Use Cases</h2>
  <ul>
    <li>Dynamic theme engines</li>
    <li>Dark/light mode transformation logic</li>
    <li>Design system experimentation</li>
    <li>Color theory learning tool</li>
    <li>Frontend interview demo project</li>
  </ul>

  <h2>Why This Project?</h2>
  <p>
    Modern UI systems often rely on runtime color adjustments.
    Instead of manually tweaking values, this demo shows how
    colors can be mathematically analyzed and transformed.
  </p>

  <p><strong>Without Programmatic Conversion:</strong></p>
  <pre>
  /* Manual trial and error */
  background-color: #2a65ff;
  background-color: #3c74ff;
  background-color: #517fff;
  </pre>

  <p><strong>With HSL Calculation:</strong></p>
  <pre>
  const adjustedHue = baseHue + 25;
  const adjustedLightness = baseLightness + 10;
  </pre>

  <p>
    This approach allows dynamic color generation based on logic,
    instead of guesswork.
  </p>

  <h2>Tech Stack</h2>
  <pre>☑ HTML5</pre>
  <pre>☑ CSS3</pre>
  <pre>☑ Vanilla JavaScript (ES6)</pre>
  <pre>☑ HSL Color Model</pre>

  <h2>Project Structure</h2>
  <pre>
  dynamic-hue-adjustment/
  └colorPicker.html
  </pre>

  <h2>Build Status</h2>
  <p>
    This is a static demonstration project and does not require a build step.
    Simply open <code>index.html</code> in any modern browser.
  </p>

  <h2>License</h2>
  <p>
    Licensed under the <a href="LICENSE">MIT License</a>.
  </p>
</section>
