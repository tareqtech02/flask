
2. **Add the JavaScript function for copying to clipboard:**

```html
```html
<script>
  function copyToClipboard(elementId) {
    var copyText = document.getElementById(elementId);
    var textArea = document.createElement("textarea");
    textArea.value = copyText.textContent;
    document.body.appendChild(textArea);
    textArea.select();
    document.execCommand('copy');
    document.body.removeChild(textArea);
    alert("Code copied to clipboard!");
  }
</script>

```python
print("Hello, World!")
