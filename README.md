 # 題目：問朋友一起玩
 你願意成為我的雙排夥伴嗎？

- 設計理念: 簡單
- 目標跟風格: 有趣、幽默

## Code
 ### `index.html` ：詢問初始問題的主頁。

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Will you be my duo</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
<div class="container">
    <div class="tenor-gif-embed"
         data-postid="19557551"
         data-share-method="host"
         data-aspect-ratio="1.20755"
         data-width="100%"><a href="https://tenor.com/view/incredibles-glasses-gif-19557551">Incredibles Glasses GIF</a>from
        <a href="https://tenor.com/search/incredibles-gifs">Incredibles GIFs</a></div> <script type="text/javascript" async src="https://tenor.com/embed.js"></script>
    <h1>Will you be my duo?</h1>
    <p> Carry me or i will tell your mom that you fail the test</p>

    <div class="button">
        <a href="yes.html" class="btn">Yes</a>
        <a href="no.html" class="btn">No</a>
    </div>
</div>
</body>
</html>

```
### `yes.html`：如果用戶在主頁上點擊「Yes」，會顯示此頁面。

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Will you be my duo</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
<div class="container">
    <div class="tenor-gif-embed" data-postid="14541252724119373531" data-share-method="host" data-aspect-ratio="1.12717" data-width="100%"><a href="https://tenor.com/view/nebsgoodtakes-incredibles-mr-incredible-fortnite-gif-14541252724119373531">Nebsgoodtakes Incredibles GIF</a>from <a href="https://tenor.com/search/nebsgoodtakes-gifs">Nebsgoodtakes GIFs</a></div> <script type="text/javascript" async src="https://tenor.com/embed.js"></script>
    <h1>YESSIR OVERNIGHT RANK!!!!!</h1
</div>


</body>
</html>
```
### `no.html`：如果用戶在主頁上點擊「No」，會顯示此頁面。

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Will you be my duo</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
<div class="container">
  <div class="tenor-gif-embed" data-postid="24136804" data-share-method="host" data-aspect-ratio="0.990625" data-width="100%"><a href="https://tenor.com/view/2021-gif-24136804">2021 Meme</a>from <a href="https://tenor.com/search/2021-memes">2021 Memes</a></div> <script type="text/javascript" async src="https://tenor.com/embed.js"></script>
  <h1>Are you sure about that</h1>


  <div class="button">
    <a href="yes.html" class="btn">Yes</a>
    <a href="no1.html" class="btn">No</a>
  </div>
</div>

</body>
</html>
```

### `no1.html`：如果用戶在 `no.html` 頁面上點擊「No」，會顯示此頁面。

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Will you be my duo</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
<div class="container">
  <div class="tenor-gif-embed" data-postid="25367396" data-share-method="host" data-aspect-ratio="2.42424" data-width="2000%"><a href="https://tenor.com/view/incredibles-incredibles-boss-incredibles-boss-throw-mr-incredible-mr-incredibles-throws-boss-gif-25367396">Incredibles Incredibles Boss GIF</a>from <a href="https://tenor.com/search/incredibles-gifs">Incredibles GIFs</a></div> <script type="text/javascript" async src="https://tenor.com/embed.js"></script>
  <h1>STILL NO ?</h1>

  <div class="button">
    <a href="yes.html" class="btn">Yes</a>
    <a href="no2.html" class="btn">No</a>
  </div>
</div>

</body>
</html>
```

### `no2.html`：如果用戶在 `no1.html` 頁面上點擊「No」，會顯示此頁面。

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Will you be my duo</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
<div class="container">
  <div class="tenor-gif-embed" data-postid="24866145" data-share-method="host" data-aspect-ratio="0.9625" data-width="100%"><a href="https://tenor.com/view/cool-gif-24866145">Cool Meme</a>from <a href="https://tenor.com/search/cool-memes">Cool Memes</a></div> <script type="text/javascript" async src="https://tenor.com/embed.js"></script>
  <h1>IM GONNA TELL YOUR GF THAT YOU CHEATED</h1>

  <div class="button">
    <a href="yes.html" class="btn">Yes</a>
    <a href="#" id="move-random" class="btn">No</a>
  </div>
</div>
<script>
  document.addEventListener('DOMContentLoaded', () => {
    const moveRandom = document.getElementById('move-random');
    const gifContainer = document.querySelector('.tenor-gif-embed');
    moveRandom.addEventListener('mouseover', () => {
      const maxX = gifContainer.offsetWidth - moveRandom.offsetWidth;
      const maxY = gifContainer.offsetHeight - moveRandom.offsetHeight;
      const x = Math.random() * maxX;
      const y = Math.random() * maxY;
      moveRandom.style.position = 'absolute';
      moveRandom.style.left = `${x}px`;
      moveRandom.style.top = `${y}px`;
    });
  });
</script>
</body>
</html>
```

### `style.css`：樣式文件，用於設計頁面。

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Montserrat', sans-serif;
}

body {
    width: 100%;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #F5F5DC;
    position: relative;
}

.container {
    display: flex;
    flex-direction: column;
    text-align: center;
    align-items: center;
    gap: 20px;
    max-width: 500px;
    margin: 20px;
}

.container .tenor-gif-embed {
    max-width: 500px;
}

.container .button {
    display: flex;
    gap: 25px;
    position: relative;
}

.button a {
    text-decoration: none;
    color: #fff;
    background-color: #000;
    padding: 10px 20px;
    border-radius: 5px;
    box-shadow: 0.5rem 1rem 3rem hsl(0, 0%, 0%, 0.3);
    position: relative;
}

```
# GIF
![GIF](https://github.com/user-attachments/assets/2556f539-ed35-4a23-ab39-4f6c4c11ef9f)
![GIF](https://github.com/user-attachments/assets/e02b5434-5a04-4732-9418-ec176e1318f2)
![GIF](https://github.com/user-attachments/assets/cd2e4126-0a58-445d-b4cc-2465dd1d5efb)
![GIF](https://github.com/user-attachments/assets/72b61baf-e303-491a-bccf-9030e5db2753)
![GIF](https://github.com/user-attachments/assets/ff5cb1b4-a7c8-4b01-b3e6-f54f4dea8310)

# Commit
![image](https://github.com/user-attachments/assets/00ec78dd-33c9-43d2-974f-0db0743c4a07)



