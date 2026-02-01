# Valentine's Day Proposal Page

A cute interactive webpage to ask someone to be your valentine.

## Usage

The name is encoded in base64 to keep it hidden in the URL.

### Step 1: Encode the name

In terminal:
```bash
echo -n "Name" | base64
```

Or use an online base64 encoder.

### Step 2: Add to URL

```
index.html?n=ENCODED_NAME
```

### Example

For "Sarah":
```bash
echo -n "Sarah" | base64
# Output: U2FyYWg=
```

URL: `index.html?n=U2FyYWg=`

### GitHub Pages

```
https://username.github.io/valentine/?n=U2FyYWg=
```
