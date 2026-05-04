# These are all for classlink.dev

It works by having code in htmlplayground. That scraps the code in index.html. And in there the apps do the exact same thing. For example, DriveMad. It scraps the code from "Drivemading.html" And for eaglercraft it scrapes the loader.html in the eaglercraft folder.

## Why this?

Well, due to the rise of the **spyware** like GoGuardian. Which just ends up restricting students freedom and privacy. Even in some cases it blocks kids from getting mental/physical help. That is a real thing that happened with securely. Securely blocked a website which would let a student if they had problems at home, could call for help. But, Securely blocked that website. What if a student that didn't have a phone needed help? How are they supposed to get the help they need? Its just a ploy that sounds good so schools get and stock price go up. Company happy.


## To get this secure html based OS. Paste this code in to [Html Playground](https://htmlplayground.com) in any of the boxes except the javascript box.

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
 ## Or, if your school doesn't have vercel blocked then go to:
https://classlink.dev
