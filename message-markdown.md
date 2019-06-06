# Markdown in messages

Deltachat is going to support the following subset of markdown:

### `*italics*`

### `**bold**`

### `~~strikethrough~~`

### `https://delta.chat` - Urls

Make URLs clickable, but **don't** support the Link syntax `[Name](url)`
because that could be used for misleading and as such be used in scams.

### `` `inline-code` ``
useful to send non markdown text in your message like source code snippets.
Should get rendered in a monospace font and with a different background.
 
### ` ``` fence code block ``` `

```
Similar to `inline-code` but not inline and it may supports code highlighting.
```
` ```[lang?] [content]``` `
 A bit modified from the common syntax to allow one liners.
 
The code **highlighting** is **optional** as implementation (time)cost 
may not be worth the small gain.
The `language` definition should be parsed separately and omitted in this case.

### `:emoji:`

## Future:

### `mailto:email@address.example.com`

Make mailto links clickable with all parameters: `?subject=Sample%20Subject&body=Sample%20Body`

### Custom Deltachat URI Scheme
see https://support.delta.chat/t/custom-deltachat-url-scheme/346

### Mentions `@username`
Clickable. (could get replaced with an user hash/email/id on send/on recieve so that it's still valid on name change.)

## Things that will not be suported:
- Inline HTML
- `[Name](url)` links
- underline - can be confused with links
