## Validate Email

```
function validateEmail(email) {
  if (/^\w+([\.-]?\w+)*@\w+([\.-]?\w+)*(\.\w{2,3})+$/.test(email)) {
    return true;
  }
  return false;
}
```
## AlphaNumeric

```
function alphaNumeric(value) {
    if (/^[0-9a-zA-Z]+$/.test(value)) {
        return true;
    }
    return false;
}
```
