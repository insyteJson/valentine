# Valentine's Day Proposal Page

A cute interactive webpage to ask someone to be your valentine.

## URL Parameters

| Parameter | Required | Description |
|-----------|----------|-------------|
| `n` | Yes | Base64 encoded recipient name |
| `k` | No | Web3Forms access key (for email notifications) |

## Quick Start

### Step 1: Encode the name

```bash
echo -n "Natsi" | base64
# Output: TmF0c2k=
```

### Step 2: Build URL

```
https://insytejson.github.io/valentine/?n=TmF0c2k=
```

## Email Notifications (Optional)

Want to know when they click "Yes"? Add email notifications:

### Step 1: Get a Web3Forms key

1. Go to https://web3forms.com
2. Enter your email
3. Copy the access key you receive

### Step 2: Add key to URL

```
https://insytejson.github.io/valentine/?n=TmF0c2k=&k=YOUR_ACCESS_KEY
```

### What you'll receive

When they click "Yes", you get an email with:
- Their name
- How many times they clicked "No" first
