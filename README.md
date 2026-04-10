# These are all for my game launcher. I did not make any of these games

It works by having code in htmlplayground. That scraps the code in index.html. And in there the apps do the exact same thing. For example, DriveMad. It scraps the code from "Drivemading.html" And for eaglercraft it scrapes the loader.html in the eaglercraft folder.

## Why this?

Well, due to the rise of the **spyware** that "Helps kids focus" when it reality it just spies on students. And blocks websites. Yes, you **should focus** but it shouldn't be forced. It should be chozen by the student. If a student doesn't pay attetion. Then they get a low grade and encourages them to work harder. But you shouldn't restrict student's rights and privacy to make them "**Focus better**". So when your done with class. Or you want to be an idiot and play games before your done. Your choice. This bypasses Spyware, and the block.

## Put this into htmlplayground.com and press preview which has a magnifying glass. And your done

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Loading...</title>
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
  html, body { height: 100%; width: 100%; overflow: hidden; background: #0a0a0a; }
  iframe { position: fixed; inset: 0; width: 100%; height: 100%; border: none; }
</style>
</head>
<body>
<iframe id="frame" sandbox="allow-scripts allow-forms allow-modals allow-popups allow-same-origin"></iframe>
<script>
  (async () => {
    const url = "https://raw.githubusercontent.com/jcdevsman/juliansgames/refs/heads/main/index.html";
    const res = await fetch(url);
    const code = await res.text();
    document.getElementById("frame").srcdoc = code;
    document.title = "Julian's Games";
  })();
</script>
</body>
</html>
```
 ## Or, if your school doesn't have github pages block then go to:
 https://jcdevsman.github.io/juliansgames/
