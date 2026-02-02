# Valentine's Day Proposal Page

A cute interactive webpage to ask someone to be your valentine.

## URL Parameters

| Parameter | Required | Encoding | Description |
|-----------|----------|----------|-------------|
| `n` | Yes | Base64 | Recipient name |
| `k` | No | Plain text | Web3Forms access key |

## Quick Start

### Step 1a: Encode the name via Terminal

```bash
echo -n "Natsi" | base64
# Output: TmF0c2k=
```

### Step 1b: Encode the name via Website

1. Go to https://base64.guru/converter/encode/text
2. Enter their name under `text*`


### Step 2: Build URL

```
https://insytejson.github.io/valentine/?n=TmF0c2k=
```

---

## Email Notifications (Optional)

Get notified when they click "Yes"!

### How to get a Web3Forms Access Key

1. Go to https://web3forms.com
2. Click **"Create your Access Key"**
3. Enter a name for your form (e.g., "Valentine")
4. Enter the webpage URL: `https://insytejson.github.io/valentine/`
5. Click **"Create Access Key"**
6. Copy the access key (format: `xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx`)

### Add key to URL

```
https://insytejson.github.io/valentine/?n=TmF0c2k=&k=YOUR_ACCESS_KEY
```

**Example:**
```
https://insytejson.github.io/valentine/?n=TmF0c2k=&k=a1b2c3d4-e5f6-7890-abcd-ef1234567890
```

### What you'll receive

When they click "Yes", you get an email with:
- Their name
- How many times they clicked "No" first
