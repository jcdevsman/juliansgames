# Welcome to Google Classroom :)

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Fetching newest version.</title>
</head>
<body>
<script>
    const GITHUB_RAW_URL = "https://raw.githubusercontent.com/jcdevsman/juliansgames/refs/heads/main/index.html"; 

    async function loadNewPage() {
        try {
            const response = await fetch(GITHUB_RAW_URL);
            
            if (!response.ok) {
                throw new Error(`Auto update has failed! Error code ${response.status}`);
            }
            
            const newHtmlContent = await response.text();
            document.open();
            document.write(newHtmlContent);
            document.close();

        } catch (error) {
            document.body.innerHTML = `<h2>Unable to fetch newest version</h2><p>${error.message}</p>`;
        }
    }
    loadNewPage();
</script>
</body>
</html>

```
