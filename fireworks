<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Fireworks Demo</title>
  <style>
    html, body {
      margin: 0;
      height: 100%;
      overflow: hidden;
      background-color: #000;
    }
    canvas {
      display: block;
    }
  </style>
</head>
<body>

<script type="module">
  import { Fireworks } from 'https://cdn.skypack.dev/fireworks-js';

  // Gắn fireworks vào body
  const container = document.body;

  // Tùy chỉnh options
  const fireworks = new Fireworks(container, {
    hue: {
      min: 0,
      max: 360
    },
    delay: {
      min: 15,
      max: 30
    },
    speed: 2,
    acceleration: 1.05,
    friction: 0.97,
    gravity: 1.5,
    particles: 50,
    trace: 3,
    explosion: 5,
    autoresize: true,
    brightness: {
      min: 50,
      max: 80,
      decay: {
        min: 0.015,
        max: 0.03
      }
    },
    boundaries: {
      top: 50,
      bottom: container.clientHeight,
      left: 50,
      right: container.clientWidth
    },
    sound: {
      enabled: false,
      files: [
        'explosion0.mp3',
        'explosion1.mp3',
        'explosion2.mp3'
      ],
      volume: {
        min: 4,
        max: 8
      }
    }
  });

  // Bắt đầu bắn pháo hoa
  fireworks.start();

  // Tự động dừng sau 10 giây
  setTimeout(() => {
    fireworks.stop();
  }, 10000);
</script>

</body>
</html>
