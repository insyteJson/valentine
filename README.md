# Valentine's Day Proposal Page

A cute interactive webpage to ask someone to be your valentine.

## URL Parameters

| Parameter | Required | Description |
|-----------|----------|-------------|
| `n` | Yes | Base64 encoded recipient name |
| `em` | No | Base64 encoded email for notification |

## Usage

### Step 1: Encode values

```bash
# Encode name
echo -n "Natsi" | base64
# Output: TmF0c2k=

# Encode email (optional)
echo -n "you@email.com" | base64
# Output: eW91QGVtYWlsLmNvbQ==
```

### Step 2: Build URL

**Without email notification:**
```
https://insytejson.github.io/valentine/?n=TmF0c2k=
```

**With email notification:**
```
https://insytejson.github.io/valentine/?n=TmF0c2k=&em=eW91QGVtYWlsLmNvbQ==
```

## Email Notification

When `em` parameter is provided:
- You'll receive an email when they click "Yes"
- Email includes how many times they clicked "No" first

**Note:** First time using your email, you'll get a confirmation email from formsubmit.co to verify your address.
